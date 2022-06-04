<template>
  <simple-memo bgColor="orange">オレンジ</simple-memo>
  <simple-memo bgColor="pink">ピンク</simple-memo>
  <simple-memo bgColor="green">みどり</simple-memo>
  <simple-memo v-bind:bgColor="inputColor">あなたの入力した色</simple-memo>
  <div>
    <span>変えてみて</span>
    <input type="text" v-model="inputColor" />
  </div>
</template>

<script>
import SimpleMemo from "./components/SimpleMemo.vue"
export default {
  components: { SimpleMemo },
  data() {
    return {
      inputColor: "black",
    }
  },
}
</script>
