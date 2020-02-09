<template>
  <div>
    <a-modal
      :visible="modalVisible"
      title="新增"
      @cancel="handleCancel"
      @ok="handleOk"
      >新增数据</a-modal
    >
    <slot />
  </div>
</template>

<script>
export default {
  data() {
    return {
      modalVisible: false
    };
  },
  methods: {
    handleClick() {
      this.modalVisible = true;
    },
    handleCancel() {
      this.modalVisible = false;
      this.$emit("callback", false);
    },
    handleOk() {
      this.modalVisible = false;
      this.$emit("callback", true);
    }
  }
};
</script>
