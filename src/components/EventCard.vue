<template>
  <div class="event-card">
    <span>@{{ event.time }} on {{ event.date }}</span>
    <h4>{{ event.title }}</h4>
  </div>
</template>

<script>
export default {
  name: 'EventCard',
  props: {
    event: Object,
  },
}
</script>
<style scoped>
.event-card {
  padding: 20 px;
  width: 250 px;
  cursor: pointer;
  border: 1px solid black;
  margin-top: 18px;
}
</style>
