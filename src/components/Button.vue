<template>
  <div>
    <a><i :class="btnClass"></i></a>
    <p>{{ btnText }}</p>
  </div>
</template>

<script>
export default {
  name: 'button',
  props: ['btnText', 'btnClass'],
}
</script>


<style lang='scss' scoped>
@import '~scss/variables.scss';
div {
  display: inline-block;
}
a {
  display: inline-block;
  position: relative;
  background-color: $green;
  padding: 1em;
  height: 1em;
  width: 1em;
  border: 3px solid white;
  border-radius: 50%;
  font-size: 1.4rem;
  line-height: 1.2em;
  color: white;
  transition: all 0.2s ease-in-out;
  box-shadow: none;
  top: 0px;
  &:hover {
    box-shadow: 0px 6px 18px rgba($darkGray, 0.4);
    top: -1px;
  }
}
i {
  font-size: 1em;
}
p {
  text-align: center;
  margin: 0.5rem 0 0 0
}
</style>
