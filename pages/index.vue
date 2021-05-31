<template>
  <div>
    <h1>Events</h1>
  </div>
</template>

<script>
export default {
  // property udes by vue-meta
  head() {
    return {
      title: "Event Listing"
    };
  },
  asyncData({ $axios }) {
    return $axios.get("http://localhost:3000/events").then(response => {
      return {
        events: response.data
      };
    });
  }
};
</script>
