<template>
  <div class="tdesign-demo-item--datepicker">
    <t-date-picker mode="date" :value="value" @change="handleChange" />
  </div>
</template>

<script lang="jsx">
import dayjs from 'dayjs';

export default {
  data() {
    return {
      value: dayjs().toISOString(),
    };
  },
  methods: {
    handleChange(value) {
      this.value = value;
    },
  },
};
</script>
