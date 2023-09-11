<script>
import Button from './components/button.vue';
export default {
  components: {
    Button
  }
}
</script>

<template>
  <div class="headerContainer">
    <div class="header">
      <div class="menu">
        <p>Item1</p>
      </div>
      <div class="menu">
        <p>Item2</p>
      </div>
      <div class="menu">
        <p>Item3</p>
      </div>
      <div class="menu-last">
        <p>Item4</p>
      </div>

    </div>
  </div>
  <div class="content">
    <div class="leftBar">
      <a href="#" class="menuLeft">Item1</a>
      <a href="#" class="menuLeft">Item2</a>
      <a href="#" class="menuLeft">Item3</a>
      <a href="#" class="menuLeft">Item4</a>
    </div>
    <div class="mainContent">
      <Button>
        <template v-slot:botao1>
          nome
        </template>
        <template v-slot:botao2>
          sobrenome
        </template>


      </Button>

    </div>
    <div class="rightBar">

    </div>
  </div>
  <div class="footer"></div>
</template>

<style scoped>
@import "@/assets/main.scss";
</style>
