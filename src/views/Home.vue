<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

interface ages { 
  [index:string]:number 
} 
const b: ages['aaa'] = 123
const a: ages[2] = 123
console.log(a)

@Component({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>
