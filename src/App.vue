<template>
  <h1>Food</h1>
  <food-item food-name="Apples" v-bind:isFavourite="true"/>
  <food-item food-name="Bananas" v-bind:isFavourite="true"/>
  <food-item v-bind:isFavourite="false"/>
</template>

<script></script>

<style>
  #app > div {
    border: dashed black 1px;
    display: inline-block;
    margin: 10px;
    padding: 10px;
    background-color: lightgreen;
  }

  #app > div:hover {
    cursor: pointer;
  }
</style>