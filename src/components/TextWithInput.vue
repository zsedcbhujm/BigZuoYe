<template>
  <div class="textwithinput">
    <a class="font">{{ font }}</a>
    <el-input
      v-model="input"
      :placeholder="content"
      :disabled="true"
    ></el-input>
  </div>
</template>

<script>
export default {
  props: {
    font: {
      type: String
    },
    content: {
      type: String
    }
  },
  data() {
    return {
      input: ""
    };
  }
};
</script>

<style lang="scss" scoped>
.textwithinput {
  padding: 5px;
}
.font {
  float: left;
  padding: 5px;
}
.el-input {
  float: right;
  width: 60%;
}
</style>
