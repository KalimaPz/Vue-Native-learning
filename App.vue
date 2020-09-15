<template>
  <view class="container">
    <text class="text-color-primary">My Vue Native App</text>
    <text>Hello Phone</text>
    <text>{{ count }}</text>
    <text>{{ name }}</text>
    <view>
      <button
        title="Increase"
        :on-press="increment"
      />
      <text-input
      :style="{height : 40 , width : 80}"
      v-model="name"
      />
    </view>
  </view>
</template>
<script>
export default {
  data() {
    return {
      count : 0,
      name : ''
    }
  },
  methods: {
    increment() {
      this.count++
    }
  },
}
</script>
<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>
