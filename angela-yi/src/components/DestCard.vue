<template>
    <div>
        <DestCard
      v-for="destination in destinations"
      :key="destination.name"
      :Destination="destination"
    />
    </div>
</template>
<script>
const destinations = [

]
</script>