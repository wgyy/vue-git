<template>
  <div>
    <div class="test"></div>
    <div class="test2"></div>
    <div class="example"></div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@svg square {
    @rect {
        fill: var(--color, black);
        width: 100%;
        height: 100%;
    }
}
.test{
  width:750px;
  height:100px;
  background: #000;
}
.test2{
  margin-top:10px;
  background: black svg(square param(--color #000));
}
@svg square {
    @rect {
        fill: var(--color, black);
        width: 100%;
        height: 100%;
    }
}
.example {
    background: white svg(square param(--color #00b1ff));
}
</style>
