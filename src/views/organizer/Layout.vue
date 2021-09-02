<template>
  <div v-if="GStore.organizer">
    <h1>{{ GStore.organizer.name }}</h1>
    <div id="nav">
      <router-link :to="{ name: 'OrganizerDetails' }">Details</router-link>
      |
      <router-link :to="{ name: 'OrganizerRegister' }">Register</router-link>
      |
      <router-link :to="{ name: 'OrganizerEdit' }">Edit</router-link>
    </div>
    <router-view :organizer="GStore.organizer" />
  </div>
</template>
<script>
export default {
  inject: ['GStore']
}
</script>
