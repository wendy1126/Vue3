<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="myFunction">클릭</button>
    <button @click="changData">변경</button>
    <br />
    <input type="text" v-model="num1" /> +
    <input type="text" v-model="num2" /> =
    <span>{{ num1 + num2 }}</span>
    <br />
    <input type="text" v-model.number="num3" /> +
    <input type="text" v-model.number="num4" /> =
    <span>{{ num3 + num4 }}</span>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'nono.go',
      num1: 0,
      num2: 0,
      num3: 0,
      num4: 0
    }
  },
  beforeCreate() {},
  created() {},
  beforeMount() {},
  mounted() {},
  beforeUpdate() {},
  updated() {},
  beforeUnmount() {},
  unmounted() {},
  methods: {
    myFunction() {
      console.log(this.userId)
    },
    changData() {
      this.userId = 'world'
    }
  }
}
</script>
