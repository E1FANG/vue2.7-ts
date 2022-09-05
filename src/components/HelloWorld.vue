<script setup lang="ts">
import { onMounted, ref } from 'vue';

type countObj ={
  count:number
  dec:string
}

const count = ref<countObj>();

onMounted(() => {
  count.value = {
    count: 123,
    dec: 'lidshfkjlasd',
  };
});
</script>

<template>
<div>
  {{count?.count}}
</div>
</template>

 <style lang="scss" scoped>

</style>
