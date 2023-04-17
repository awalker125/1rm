<script>
export default {
  data() {
    return {
      reps: 1,
      weight: 100,
    }
  },
  computed: {
    max() {
      //=D2233*(1+E2233*0.033)
      let _max = this.weight * (1 + this.reps * 0.033);
      return _max.toFixed(2) + "kg"


    }
  }
}
</script>

<template>
  <div class="calculator">


    <h1>
      <span>{{ max }}</span>
    </h1>

    <label for="kgs">kgs</label>
    <input id="kgs" type="text" v-model="weight" />
    <label for="reps">Reps</label>
    <input id="reps" type="text" v-model="reps" />

  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.calculator h1,
.calculator h3 {
  text-align: center;
}

@media (min-width: 1024px) {

  .calculator h1,
  .calculator h3 {
    text-align: left;
  }
}

label {
  display: block;
  margin-bottom: 10px;
}
</style>
