<template>
  <div id="box">
    <!-- title区域 -->
    <Title></Title>
    <!--  tool区域  -->
    <div class="tools">
      <div class="left">
        <span class="toolLeft"></span>
      </div>
      <div class="right">
        <span class="toolRight1"></span>
        <span class="toolRight2"></span>
      </div>
    </div>
    <!-- content区域 -->
    <table class="content">
      <thead>
        <tr class="head">
          <th>一</th>
          <th>二</th>
          <th>三</th>
          <th>四</th>
          <th>五</th>
          <th>六</th>
          <th>日</th>
        </tr>
      </thead>
    </table>
    <!-- <div class="slideHeight">
      <div class="slideshow"></div>
    </div> -->
    <!-- navigation区域 -->
    <!-- <div class="nav">
      <div class="navshow"></div>
    </div> -->
  </div>
</template>

<script>
import "./calendar.css";
import Title from "./Title.vue";
export default {
  components: {
    Title,
  },
  data() {
    return {};
  },
};
</script>

<style lang="less" scoped>
</style>