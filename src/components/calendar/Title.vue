<template>
  <div class="title">
    <div class="titleTime">{{ strTime }}</div>
    <div class="titleData">{{ strDate }}</div>
  </div>
</template>

<script>
import { lunarCalendar, solarCalendar } from "@/common/utils.js";
export default {
  data() {
    return {
      strTime: undefined,
      strDate: undefined,
    };
  },
  mounted() {
    this.init();
  },
  methods: {
    //   标题初始化
    init() {
      let today = new Date();
      let yyTitle = today.getFullYear(); // 年
      let moTitle = today.getMonth() + 1; // 月
      let ddTitle = today.getDate(); // 日
      let hhTitle = today.getHours(); // 时
      let mmTitle = today.getMinutes(); // 分
      let ssTitle = today.getSeconds(); // 秒
      this.strTime =
        this.handleFormat(hhTitle) +
        ":" +
        this.handleFormat(mmTitle) +
        ":" +
        this.handleFormat(ssTitle);
      this.strDate =
        yyTitle +
        "年" +
        moTitle +
        "月" +
        ddTitle +
        "日" +
        lunarCalendar.get(moTitle) +
        "月" +
        solarCalendar.get(ddTitle) +
        "日";
      let timeID = setInterval(() => {
        this.init();
        clearInterval(timeID);
      }, 1000);
    },
    handleFormat(a) {
      // 数字是个位数的话,前面要加0 十位就不用加
      return a < 10 ? "0" + a : a;
    },
  },
};
</script>

<style lang="scss" scoped>
</style>