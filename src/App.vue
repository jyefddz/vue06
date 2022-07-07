<template>
  <div>
    <UseTable>
      <template v-slot:name="scope">
        <input v-model="scope.row.name">
      </template>
      <template v-slot:age="scope">
        <input v-model="scope.row.age">
      </template>
      <template v-slot:toux="scope">
        <a v-if="scope.row.type == 0" :href="scope.row.headImgUrl">{{ scope.row.headImgUrl }}</a>
        <img v-else-if="scope.row.type == 1" :src="scope.row.headImgUrl" alt="">
        <span v-else>{{ scope.row.headImgUrl }}</span>
      </template>
    </UseTable>
    <br>
    <hr>
    <br>
    <UserInfo></UserInfo>

  </div>
</template>

<script>
import UseTable from './components/01/01_UseTable.vue'
import UserInfo from './components/UserInfo.vue'
export default {
  data() {
    return {
    }
  },
  components: {
    UseTable,
    UserInfo,
  },
  computed: {
  }
}
</script>

<style>
</style>