<script setup>
import InputText from 'primevue/inputtext';
import Button from 'primevue/button';
import { ref } from 'vue';

const text = ref('');

const num = ref(0);

const num2 = ref(5);

// function addone() {
//   num.value = num.value +  1;
//   console.log(num.value);
// }

const addone = () => {
  num.value = num.value + num2.value;
  console.log(num.value);
}
</script>

<template>
  <div>
    <InputText v-model="num2"/>
    {{ num2 }}
    
  </div>
  <div>
    <Button @click="addone">Add</Button>
    <p>Current number: {{ num }}</p>
    
  </div>
</template>

