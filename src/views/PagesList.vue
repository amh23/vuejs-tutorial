<template>
    <p>{{ counter }}</p>
    <button @click.prevent="click">Click</button>
</template>
<script setup>
import { ref, reactive } from 'vue';

const counter = ref(0); // {value: 0}

function click(){
    counter.value++;
}
// export default{
//     data(){
//         return {
//             counter: 0
//         };
//     },
//     methods: {
//         click(){
//             this.counter++;
//         }
//     }
// }
</script>
