<template>
  <div class='icon-wrapper'>
    <svg class="icon" :width="width" :height="height">
      <use v-bind="{'xlink:href':'/feather-sprite.svg#'+name}" />
    </svg>
    <slot></slot>
  </div>
</template>

<script>
  export default {
    props: {
      name:String,
      width: {
        type: [Number, String],
        default: 24
      },
      height: {
        type: [Number, String],
        default: 24
      },
    },
  }
</script>

<style scoped>
.event-card {
  padding: 20px;
  margin-bottom: 24px;
  transition: all 0.2s linear;
  cursor: pointer;
}
.event-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2), 0 1px 15px 0 rgba(0, 0, 0, 0.19);
}
.event-card > .title {
  margin: 0;
}
.event-link {
  color: black;
  text-decoration: none;
  font-weight: 100;
}
</style>