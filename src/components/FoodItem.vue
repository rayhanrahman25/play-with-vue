<template>
    <div v-on:click="countClicks">
      <h2>{{ foodName }}</h2>  
      <img v-show="isFavourite" src="https://www.w3schools.com/vue/img_quality.svg" height="50" alt="">
      <p id="red">You have clicked me {{ clicks }} times.</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        message: 'I like apples',
        clicks: 0,
      }
    },
    props: {
      foodName: {
        type: String,
        required: true,
        default: 'Not Set',
      },
      isFavourite: Boolean
    },
    methods: {
      countClicks() {
        this.clicks++;
      }
    }
  }
  </script>
  
  <style>
    #red {
      font-weight: bold ;
      color: rgb(144, 12, 12);
    }
  </style>