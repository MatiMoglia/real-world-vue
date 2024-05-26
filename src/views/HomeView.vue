<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="home">
    <EventCard />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  components: {
    EventCard,
  },
}
</script>
