<template>
  <div>
    <input
      type="search"
      name=""
      id=""
      @keyup="checkEnter($event)"
      v-model="searchText"
    />
    <button @click="doSearch">조회</button>
    <input
      type="search"
      name=""
      id=""
      @keyup.enter="doSearch"
      v-model="searchText"
    />
    <button @click="doSearch">조회</button>
    <button type="submit" @click.prevent="doSearch">submit</button>
  </div>
</template>
<script>
// .enter
// .tab
// .delete
// .esc
// .space
// .up
// .down
// .left
// .right
// .ctrl
// .stop - event.stopPropagetion()
// .prevent - event.preventDefault();
// 키 이벤트를 바로 호출할 수 있음
export default {
  components: {},
  data() {
    return {
      example: ''
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
    doSearch() {
      console.log(this.searchText)
    },
    checkEnter(event) {
      if (event.keyCode === 13) {
        this.doSearch()
      }
    }
  }
}
</script>
