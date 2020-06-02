<template>
  <div id="app">
    <h1>Hosting Price</h1>
    <h2>호스팅 비용 안내</h2>
    <p>
      Vue119는 CMS, Netlify 기반의 컨텐츠 관리 시스템을 적용하여 보다 편하게
      홈페이지를 관리할 수 있도록 도와드립니다.
    </p>
    <table>
      <tr>
        <td v-for="type in types" :key="type">{{ type }}</td>
      </tr>
      <tr>
        <td v-for="plan in plans" :key="plan">{{ plan }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {}
};
</script>
<style scoped lang="scss">
h1 {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 22px;
}
</style>
