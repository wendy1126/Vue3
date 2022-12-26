<template>
  <div>
    <h1>Hello {{ userName }}</h1>
    <p>{{ message }}</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      userName: 'John Doe',
      message: 'Welcome to 해원 world'
    }
  }
}
</script>
<style scoped>
/*전체 적용하기 위해 만든 스타일(주로 assets폴더에 css 파일 생성함) 외에
해당 화면에만 적용해야 할 새로운 스타일은 <style scoped>에 작성*/
</style>
