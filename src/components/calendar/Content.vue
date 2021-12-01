<template>
  <div></div>
</template>

<script>
export default {
  data() {
    return {};
  },
  mounted() {
    this.init();
  },
  methods: {
    //   内容初始化
    init() {
    //   //根据当前需要显示的年和月来创建日历
    //   //创建一个要显示的年月的下一个的日期对象
    //   let date1 = new Date(y, m, 1, 0, 0, 0);
    //   //对下一个月的1号0时0分0秒的时间 - 1得到要显示的年月的最后一天的时间
    //   let date2 = new Date(date1.getTime() - 1);
    //   //得到要显示的年月的总天数
    //   let showMonthDays = date2.getDate();
    //   date2.setDate(1);
    //   //获取要显示的年月的1日的星期,从0开始的星期
    //   //showMonthWeek表示这个月的1日的星期，也可以作为表格中前面空白的单元格的个数
    //   let showMonthWeek = date2.getDay(); // 5
    //   if (showMonthWeek === 0) showMonthWeek = 7;
    //   let cells = 7;
    //   let rows = 6; // 由于windows上面的日历始终显示7行，所以固定为6

    //   // 这里要那当前显示月份的上一个月有多少天，以及拿当前显示月份的下一月有多少天
    //   let datePre = new Date(y, m - 1, 0, 0, 0, 0);
      //   // 前面需要补 showMonthWeek - 1 个
      //   let datePreDates = showMonthWeek - 1;

      //   let dateNext = new Date(y, m + 1, 0, 0, 0, 0);
      //   // 后面需要补 showMonthWeek - 1 + showMonthDays 个
      //   let dateNextDates = showMonthWeek - 1 + showMonthDays;
    },
  },
};
</script>

<style lang="scss" scoped>
</style>