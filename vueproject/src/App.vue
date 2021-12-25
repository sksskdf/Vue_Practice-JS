<template>
  <div> <!-- 템플릿 바로 밑에는 하나의 태그만 존재해야 에러가 안남-->
    <h1>{{ title }}</h1> <!-- 데이터 바인딩-->
    <p>{{ count }}</p>
    <button @click="count ++">추가</button>
  </div>
</template>

<script>
  export default {
    data() {
      return{
        title:"안녕하세요.",
        count : 1
      }
    }
  }
</script>
