<template>
  <div>
    <van-picker
      v-if="flag"
      :columns="columns"
      @change="changePicker"
    />
    <van-button @click="show">显示</van-button>
  </div>

</template>

<script>
export default {
  data() {
    return {
      columns: ["杭州", "宁波", "温州", "嘉兴", "湖州"],
      flag: false
    };
  },
  methods: {
    show() {
      console.log("1 =", "show");
      this.flag = !this.flag;
    },
    changePicker(event) {
      console.log("1 =", event);
    }
  }
};
</script>
