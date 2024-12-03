<template>

  <div class="page">
    <h1 style="margin-top: 120px; text-align: center;">Gas vs. Electric</h1>
    <p>This calculator compares how many tons of emissions are released by gas and electric cars per month. On average, gas cars are responsible for releasing <a target="_blank" href="https://www.epa.gov/greenvehicles/greenhouse-gas-emissions-typical-passenger-vehicle#:~:text=typical%20passenger%20vehicle%3F-,A%20typical%20passenger%20vehicle%20emits%20about%204.6%20metric%20tons%20of,8%2C887%20grams%20of%20CO2.">4.6 tons</a> of emissions per year. In contrast, electric vehicles are responsible for an averge of <a href="https://usafacts.org/articles/how-much-emissions-do-electric-cars-produce/" target="_blank">1.9 tons</a> of emissions per year due to electricity production. Use the calculator to see how these numbers compare at scale.</p>
    <br>

    <!-- Average fuel cost -->
     <label for="num">Number of cars</label>
    <input name="num" type="text" v-model="carNum">
    <label style="margin-top: 8px;" for="gas">Months driving</label>
    <input name="months" type="text" v-model="months">
    <br>
    <p><strong>Gas emissions (tons): </strong>{{ gasEmissions }}</p>
    <p><strong>Electric emissions (tons): </strong>{{ electricEmissions }}</p>
    <br>
    <p style="font-size: 1.8vw"><strong>Gas cars save: </strong>{{ parseInt((gasEmissions - electricEmissions) * 100) / 100 }} tons</p>
  </div>
</template>

<script>
export default {
  name: 'calculator',
  data() {
    return {
      months: 0,
      carNum: 1,
      gasTonsPerMonth: 0.383,
      electricTonsPerMonth: 0.16,
    }
  },
  computed: {
    gasEmissions() {
      return parseInt(this.carNum * (this.gasTonsPerMonth * this.months) * 100) / 100;
    },
    electricEmissions() {
      return parseInt(this.carNum * (this.electricTonsPerMonth * this.months) * 100) / 100;
    }
  }
}
</script>

<style scoped>
input {
  padding: 8px;
  padding-left: 15px;
  border-radius: 2px;
  border: none;
  width: 400px;
}
input:focus {
  outline: none;
}
.page {
  display: flex;
  flex-direction: column;
  color: white;
  width: 80%;
  margin: auto;
  font-size: 2vw;
  margin-bottom: 90px;
}

h5 {
  padding: 15px;
  font-size: 1.2vw;
  margin: 0;
}
p, label, a {
  margin: 0;
  font-size: 20px;
  font-size: 1.3vw;
  color: rgba(255, 255, 255, 0.651);
}
</style>

<!-- https://ev-lectron.com/blogs/blog/electric-car-maintenance-cost#:~:text=Meanwhile%2C%20traditional%20cars%20need%20around,maintenance%20fees%20throughout%20its%20lifetime. -->

<!-- https://www.epa.gov/greenvehicles/greenhouse-gas-emissions-typical-passenger-vehicle#:~:text=typical%20passenger%20vehicle%3F-,A%20typical%20passenger%20vehicle%20emits%20about%204.6%20metric%20tons%20of,8%2C887%20grams%20of%20CO2. -->

<!-- https://usafacts.org/articles/how-much-emissions-do-electric-cars-produce/ -->