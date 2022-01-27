<template>
  <div class="relative flex items-top justify-center min-h-screen bg-gray-100 sm:items-center sm:pt-0">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.1.2/dist/tailwind.min.css" rel="stylesheet">
    <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6 card">
      <div class="image">
        <img src="https://dummyimage.com/192x128/96bee0/fff" class="thumbnail">
      </div>
      <div class="info">
        <h2 class="text-2xl leading-7 font-semibold">
          {{ title }}
        </h2>
        <p class="mt-3 text-gray-600">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras ornare sodales elit. Aenean nunc nisl, tempor et fermentum vel, viverra et libero. In eleifend et odio et pellentesque.<br>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'VideoCard',
  props: {
    title: {
      type: String,
      default: 'Video'
    }
  }
}
</script>

<style>
  .card {
    width: 100%;
    max-width: 730px;
    display: flex;
    align-items: center;
  }
  .image {
    position: relative;
    width: 100%;
    max-width: 220px;
    /* border-radius: 6px; */
    overflow: hidden;
    display: block;
    /* display: flex; */
    align-items: center;
    justify-content: center;
  }
  .thumbnail {
    height: 128px;
    border-radius: 3px;
  }
  .info {
    flex: 1;
    margin-left: 2rem;
  }
</style>
