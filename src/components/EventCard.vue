<template>
  <div class="event-card">
    <span>@{{ event.time }} on {{ event.date }}</span>
    <h4>{{ event.title }}</h4>
  </div>
</template>

<script>
export default {
  name: 'EventCard',
  //props: {
  //  msg: String,
  //},
  data() {
    return {
      event: {
        id: 1,
        title: 'Event Title',
        description: 'Event Description',
        location: 'Event Location',
        date: 'Event Date',
        time: 'Event Time',
      },
    }
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
