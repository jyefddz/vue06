<template>
  <div>
    <UseTable>
      <template v-slot:age="scope">
        <input v-model="scope.row.age">
      </template>
      <template v-slot:toux="scope">
        <a :href="scope.row.headImgUrl">{{ scope.row.headImgUrl }}</a>
      </template>
      <template v-slot:toux1="scope">
        <img :src="scope.row.headImgUrl" alt="">
      </template>
      <template v-slot:toux2="scope">
        <span>{{ scope.row.headImgUrl }}</span>
      </template>
    </UseTable>
  </div>
</template>

<script>
import UseTable from './components/01/01_UseTable.vue'
export default {
  data() {
    return {
    }
  },
  components: {
    UseTable
  },
  computed: {
  }
}
</script>

<style>
</style>