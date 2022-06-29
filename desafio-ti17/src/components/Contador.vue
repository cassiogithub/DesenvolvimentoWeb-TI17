<template >
  <h2>Contador</h2>
  <span @mousedown.left="aumentar()" @mousedown.right="diminuir()">{{
    value
  }}</span>
  <span class="instrucoes">
    Ao clicar com o botão esquerdo do mouse, deve <em>somar</em> um ao contador
  </span>
  <span class="instrucoes">
    Ao clicar com o botão esquerdo do mouse, deve <em>subtrair</em> um ao
    contador
  </span>
</template>

<script>
export default {
  name: "Contador",

  data() {
    return {
      value: 0,
    };
  },
  methods: {
    aumentar(event) {
      this.value++;
      console.log(this.value);
    },
    diminuir(event) {
      this.value--;
      console.log(this.value);
    },
  },
};
</script>
<style scoped>
span {
  font-size: 3rem;
}
button {
  display: block;
  margin: 1rem auto;
}

.instrucoes {
  display: block;
  font-size: 1rem;
}
</style>
