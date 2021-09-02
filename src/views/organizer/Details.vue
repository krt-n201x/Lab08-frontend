<template>
  <p>{{ organizer.id }}</p>
  <p>{{ organizer.name}}</p>
  <p>{{ organizer.address}}</p>
</template>

<script>
export default {
  props: ['organizer']
}
</script>
