<script setup>
import { defineModel } from 'vue';
const first= defineModel('value')
const last = defineModel('value1')
function Clear()
    {
        first.value='';
        last.value=''
    }
</script>

<template>
  <span>User Name : </span> <input v-model="first" placeholder="FirstName"> &nbsp;
  <input v-model="last" placeholder="LastName">  &nbsp; 
    <button id="button" @click="Clear()">ClearText</button>
</template>
<style>
#button:hover
{
    cursor: pointer;
    background-color: black;
    color: white;
}
</style>