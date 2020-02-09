<template>
  <div>
    <create-form-action ref="refCreateFormAction" @callback="onCallback">
      <a-button
        type="primary"
        ghost
        @click="$refs.refCreateFormAction.handleClick()"
        >新增</a-button
      >
    </create-form-action>
  </div>
</template>

<script>
import CreateFormAction from "./handle-action/create-form.vue";

export default {
  components: { CreateFormAction },
  methods: {
    handleClick() {
      // this.$refs.refCreateFormAction.handleClick();
    },
    onCallback(res) {
      console.log("callback", res);
    }
  }
};
</script>
