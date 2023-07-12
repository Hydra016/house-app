<template>
    <div>
        <h1>My Listings</h1>
        <ul>
            <li v-for="house in myListings" :key="house.id">
                {{ house.address }}
            </li>
        </ul>
    </div>
</template>
<script>
export default {
    name: 'MyListings',
    data() {
        return {
            myListings: []
        };
    },
    mounted() {
        // Fetch the user's listings from API or use Vuex store to get the data
        // Update myListings with the fetched data
    }
}
</script>

<style>
.listings-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 16px;
}

.house-card {
  flex: 1;
  min-width: 300px;
  max-width: 400px;
  /* Add additional styles for the house card */
}


</style>
  
  