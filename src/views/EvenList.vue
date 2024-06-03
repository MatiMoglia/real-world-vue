<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <h1>Events</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'
//import axios from 'axios'

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 1,
          name: 'Event 1',
          date: '2020-01-01',
          description: 'Event 1 description',
          title: 'Event 1 title',
          location: 'Event 1 location',
        },
        {
          id: 2,
          name: 'Event 2',
          date: '2020-01-02',
          description: 'Event 2 description',
          title: 'Event 2 title',
          location: 'Event 2 location',
        },
        {
          id: 3,
          name: 'Event 3',
          date: '2020-01-03',
          description: 'Event 3 description',
          title: 'Event 3 title',
          location: 'Event 3 location',
        },
      ],
    }
  },
  async created() {
    /*const response = await axios.get().then(response) => {
      this.events = response.dataevents = response.data
    }*/
  },
}
</script>
<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
