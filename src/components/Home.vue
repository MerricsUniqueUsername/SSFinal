<template>
  <div class="top" style="display: block; position: relative; top: 120px;">

    <div class="row">
      <div class="cell" style="flex-direction: column;">
        <h1 style="margin: 0; margin-top: 35px;">Driving Change, Empowering Tribal Nations</h1>
        <h2 style="margin: 0; margin-top: 8px; left: 0;">Paving the Way to Clean Energy and Stronger Communities</h2>
        <div class="button" style="margin-top: 80px; font-size: 16px; width: 160px; align-self: start;">Explore</div>
      </div>
      <div class="cell">
        <img src="../assets/Car.png" alt="">
      </div>
    </div>

    <div class="names" style="margin-top: 15px;">
      <span style="margin-left: 40px;">Merric Justian</span>
      <span>Tairen Caron</span>
      <span>Caleb Werdon</span>
      <span>Decker Hodge</span>
      <span style="margin-right: 40px;">Eli Vanvynckt</span>
    </div>

    <div class="problem" style="background-color: white; margin-top: 50px;">
      <div class="row">
        <div class="cell" style="width: 70%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 3.5vw; color: black;">Problem Statement</h1>
          <p style="font-size: 18px; opacity: 0.7; margin-bottom: 70px;">
            Throughout this project, we will be looking into the opportunities and barriers associated with bringing electric vehicle charging infrastructure to Tribal Nations in the Great Lakes region. By examining the specific needs of these communities, we can identify how EV infrastructure can support economic development, promote energy independence, and impact inequality. However, we must also address the significant regulatory and geographic challenges that may hinder EV implementation. Ultimately, this project will seek collaboration and innovation that can lead to access to EV technology while ensuring to honor of the values of tribal nations.
          </p>
        </div>

        <div class="cell" style="width: 30%; position: relative; align-self: center; overflow: hidden;">
          <div class="windmill" style="left: 0px;">
            <img src="../assets/Windmill_bottom.svg" alt="">
            <img ref="blades" style="position: absolute; left: 0; top: 5%;" src="../assets/Windmill_top.svg" alt="">
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'Home',
  methods: {

    /**
     * Animate blades rotating
     */
     animateBlades() {
      const blades = this.$refs.blades;
      blades.style.transformOrigin = '49% 36.8%';
      blades.animate([
        { transform: 'rotate(0deg)' },
        { transform: 'rotate(360deg)' }
      ], {
        duration: 3000,
        iterations: Infinity,
        easing: 'linear'
      });
    }

  },
  mounted() {
    this.animateBlades();
  }
}
</script>

<style>
  .windmill {
    position: relative;
    /* Scale up */
    transform: scale(1.4);
  }
  .names {
    color: rgba(255, 255, 255, 0.832);
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-size: 1.1vw;
    position: relative;
    padding: 15px;
    border-bottom: 1px solid rgb(29, 29, 29);
    border-top: 1px solid rgb(29, 29, 29);
  }

  .button {
    background-color: #2196F3;
    color: white;
    padding: 15px 42px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    border: none;
    cursor: pointer;
    transition: background-color 0.3s;
    border-radius: 2px;
  }
  .button:hover {
    background-color: #af4c87;
  }

  h1 {
    font-size: 4vw;
    line-height: 1;
    width: 100%;
  }
  h2 {
    font-size: 1.5vw;
    line-height: 1;
    color: rgba(255, 255, 255, 0.638);
    font-weight: 100;
    width: 100%;
  }

  /* Main container styles */
  .top {
    height: fit-content;
    width: 100vw;
  }

  /* Flex container for rows */
  .row {
    width: 85%;
    height: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap; /* Allows cells to stack on smaller screens */
    margin: auto;
    position: relative;
  }

  /* Individual cell styles */
  .cell {
    height: 100%; /* Adjust for smaller screens */
    width: 50%; /* Full width on small screens */
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    box-sizing: border-box;
    padding: 1rem; /* Adds some space inside cells */
  }

  /* Image styles */
  .cell img {
    width: 80%;
    justify-self: center;
    align-self: center;
    border-radius: 8px;
  }

  /* Media query for smaller screens */
  @media (max-width: 900px) {
    .cell {
      width: 100%; /* Side-by-side layout on medium+ screens */
      height: 50%; /* Full height */
    }
    .cell img {
      height: 100%;
    }
    .names {
      margin-top: 800px;
    }
  }
</style>
