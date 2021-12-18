<template>
  <div class="events">
    <EventCard 
      v-for="event in events" 
      :key="event.id" 
      :event="event"/>
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 3456,
          category: 'animal',
          title: 'Cat adoption',
          description: 'Find your ...',
          location: 'Town',
          date: 'Jan 21, 2021',
          time: '12:00',
          petsAlllowed: true,
          organizer: 'John Doe'
        },
        {
          id: 3456,
          category: 'animal',
          title: 'Cat adoption',
          description: 'Find your ...',
          location: 'Town',
          date: 'Jan 21, 2021',
          time: '12:00',
          petsAlllowed: true,
          organizer: 'John Doe'
        },
        {
          id: 3456,
          category: 'animal',
          title: 'Cat adoption',
          description: 'Find your ...',
          location: 'Town',
          date: 'Jan 21, 2021',
          time: '12:00',
          petsAlllowed: true,
          organizer: 'John Doe'
        },
      ],
    }
  }
};
</script>

<style scoped>
  .events {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>