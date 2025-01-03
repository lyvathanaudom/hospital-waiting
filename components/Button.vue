<template>
    <button class="bg-blue-500 text-white px-4 py-1 rounded-3xl hover:bg-blue-600">{{ text }}</button>
  </template>
  
  <script>
  export default {
    props: {
      text: {
        type: String,
        required: true,
      },
    },
  };
  </script>