<template>

  <div class="button next" :class="{'visible': scrolled > 12}">
    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-chevron-double-down" viewBox="0 0 16 16">
      <path fill-rule="evenodd" d="M1.646 6.646a.5.5 0 0 1 .708 0L8 12.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708"/>
      <path fill-rule="evenodd" d="M1.646 2.646a.5.5 0 0 1 .708 0L8 8.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708"/>
    </svg>
  </div>

  <div class="top" style="display: block; position: relative; top: 120px;">

    <div class="row">
      <div class="cell" style="flex-direction: column;">
        <h1 style="margin: 0; margin-top: 35px;">Driving Change, Empowering Tribal Nations</h1>
        <h2 style="margin: 0; margin-top: 8px; left: 0;">Paving the Way to Clean Energy and Stronger Communities</h2>
        <div class="button" style="margin-top: 80px; font-size: 16px; width: 160px; align-self: start;" @click="goToProblemPage">Explore</div>
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

    <div class="problem slide" style="background-color: white; height: 100vh">
      <div class="row">
        <div class="cell" style="width: 70%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 3.5vw; color: black;">Problem Statement</h1>
          <p style="font-size: 24px; opacity: 0.7; margin-bottom: 70px;">
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

    <div class="intro slide" style="background-color: white; height: 100vh">
      <div class="row">
        <div class="cell" style="width: 100%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 3.5vw; color: black;">Introduction</h1>
          <p style="font-size: 24px; opacity: 0.7; margin-bottom: 70px; margin-bottom: 8px">
            The Great Lakes region is home to numerous tribal nations, each with unique challenges and opportunities related to electric vehicle charging infrastructure. In this project, we explore electric vehicle charging infrastructure. This project explores:
          </p>
          <ul style="text-align: left; width: 100%; margin: 6px; margin-left: 35px; font-size: 18px; opacity: 0.7;">
            <li>How the development of EV vehicles is influenced by politics</li>
            <li>How EV technology can potentially be superior to gas-powered cars for the environment in some ways</li>
            <li>How EV infrastructure can support economic development, promote energy independence, and impact inequality</li>
            <li>The environental impact of gas-powered cars and electric cars</li>
          </ul>
          <p style="font-size: 24px; opacity: 0.7; margin-bottom: 70px;">
          </p>
        </div>
      </div>
    </div>


    <div class="perks slide" style="background-color: white; height: 100vh">
      <div class="row">
        <div class="cell" style="width: 100%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 3.5vw; color: black;">
            Perks of EVs in Rural Communities
            <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" fill="currentColor" class="bi bi-globe-americas" viewBox="0 0 16 16">
              <path d="M8 0a8 8 0 1 0 0 16A8 8 0 0 0 8 0M2.04 4.326c.325 1.329 2.532 2.54 3.717 3.19.48.263.793.434.743.484q-.121.12-.242.234c-.416.396-.787.749-.758 1.266.035.634.618.824 1.214 1.017.577.188 1.168.38 1.286.983.082.417-.075.988-.22 1.52-.215.782-.406 1.48.22 1.48 1.5-.5 3.798-3.186 4-5 .138-1.243-2-2-3.5-2.5-.478-.16-.755.081-.99.284-.172.15-.322.279-.51.216-.445-.148-2.5-2-1.5-2.5.78-.39.952-.171 1.227.182.078.099.163.208.273.318.609.304.662-.132.723-.633.039-.322.081-.671.277-.867.434-.434 1.265-.791 2.028-1.12.712-.306 1.365-.587 1.579-.88A7 7 0 1 1 2.04 4.327Z"/>
            </svg>
          </h1>
          <p style="font-size: 24px; opacity: 0.7; margin-bottom: 70px;">
            The benefits of building a network for EVs in rural and tribal areas are countless. The communities in these areas will experience economic benefits, keep a healthier environment, and allow access to better transportation for the citizens of these rural communities. Economically, EVs will allow for overall cheaper transportation, create more jobs in these areas, and increase tourism. These things will help lead to a rise in the economy of rural and tribal communities that establish an EV network. Looking at the environment, EVs will protect natural resources while also combating pollution and climate change in these communities. On top of these economic and environmental pros, EVs will also serve as a more reliable form of transportation in these rural areas with the implementation of an EV network.
          </p>
        </div>
      </div>
    </div>

    <div class="environment slide" style="background-color: white; height: 100vh">
      <div class="row">
        <div class="cell" style="width: 100%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 3.5vw; color: black;">
            Environmental Impact of Electric Vehicles
            <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" fill="currentColor" class="bi bi-flower3" viewBox="0 0 16 16">
              <path d="M11.424 8c.437-.052.811-.136 1.04-.268a2 2 0 0 0-2-3.464c-.229.132-.489.414-.752.767C9.886 4.63 10 4.264 10 4a2 2 0 1 0-4 0c0 .264.114.63.288 1.035-.263-.353-.523-.635-.752-.767a2 2 0 0 0-2 3.464c.229.132.603.216 1.04.268-.437.052-.811.136-1.04.268a2 2 0 1 0 2 3.464c.229-.132.489-.414.752-.767C6.114 11.37 6 11.736 6 12a2 2 0 1 0 4 0c0-.264-.114-.63-.288-1.035.263.353.523.635.752.767a2 2 0 1 0 2-3.464c-.229-.132-.603-.216-1.04-.268M9 4a2 2 0 0 1-.045.205q-.059.2-.183.484a13 13 0 0 1-.637 1.223L8 6.142l-.135-.23a13 13 0 0 1-.637-1.223 4 4 0 0 1-.183-.484A2 2 0 0 1 7 4a1 1 0 1 1 2 0M3.67 5.5a1 1 0 0 1 1.366-.366 2 2 0 0 1 .156.142q.142.15.326.4c.245.333.502.747.742 1.163l.13.232-.265.002a13 13 0 0 1-1.379-.06 4 4 0 0 1-.51-.083 2 2 0 0 1-.2-.064A1 1 0 0 1 3.67 5.5m1.366 5.366a1 1 0 0 1-1-1.732l.047-.02q.055-.02.153-.044.202-.048.51-.083a13 13 0 0 1 1.379-.06q.135 0 .266.002l-.131.232c-.24.416-.497.83-.742 1.163a4 4 0 0 1-.327.4 2 2 0 0 1-.155.142M9 12a1 1 0 0 1-2 0 2 2 0 0 1 .045-.206q.058-.198.183-.483c.166-.378.396-.808.637-1.223L8 9.858l.135.23c.241.415.47.845.637 1.223q.124.285.183.484A1.3 1.3 0 0 1 9 12m3.33-6.5a1 1 0 0 1-.366 1.366 2 2 0 0 1-.2.064q-.202.048-.51.083c-.412.045-.898.061-1.379.06q-.135 0-.266-.002l.131-.232c.24-.416.497-.83.742-1.163a4 4 0 0 1 .327-.4q.07-.074.114-.11l.041-.032a1 1 0 0 1 1.366.366m-1.366 5.366a2 2 0 0 1-.155-.141 4 4 0 0 1-.327-.4A13 13 0 0 1 9.74 9.16l-.13-.232.265-.002c.48-.001.967.015 1.379.06q.308.035.51.083.098.024.153.044l.048.02a1 1 0 1 1-1 1.732zM8 9a1 1 0 1 1 0-2 1 1 0 0 1 0 2"/>
            </svg>
          </h1>
          <p style="font-size: 24px; opacity: 0.7; margin-bottom: 70px;">
            Electric vehicles (EVs) are an environmentally friendly alternative to gas-powered cars, with significant benefits in reducing greenhouse gas emissions and improving public health. While their manufacturing produces higher emissions due to battery production, EVs offset this within 18 months of driving, ultimately having a smaller carbon footprint—even when charged on less clean energy grids. They are also more cost-effective over time; despite a higher initial purchase price, federal and state incentives, lower fuel costs, and reduced maintenance expenses lead to lifetime savings of $7,000 to $11,000 compared to gas vehicles. By cutting emissions and saving money, EVs offer a sustainable and economical solution to modern transportation needs.
          </p>
        </div>
      </div>
    </div>

    <div class="opportunities slide" style="background-color: white; height: 100vh">
      <div class="row">
        <div class="cell" style="width: 100%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 3.5vw; color: black;">
            Opportunities for Power
            <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" fill="currentColor" class="bi bi-battery-charging" viewBox="0 0 16 16">
              <path d="M9.585 2.568a.5.5 0 0 1 .226.58L8.677 6.832h1.99a.5.5 0 0 1 .364.843l-5.334 5.667a.5.5 0 0 1-.842-.49L5.99 9.167H4a.5.5 0 0 1-.364-.843l5.333-5.667a.5.5 0 0 1 .616-.09z"/>
              <path d="M2 4h4.332l-.94 1H2a1 1 0 0 0-1 1v4a1 1 0 0 0 1 1h2.38l-.308 1H2a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2"/>
              <path d="M2 6h2.45L2.908 7.639A1.5 1.5 0 0 0 3.313 10H2zm8.595-2-.308 1H12a1 1 0 0 1 1 1v4a1 1 0 0 1-1 1H9.276l-.942 1H12a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2z"/>
              <path d="M12 10h-1.783l1.542-1.639q.146-.156.241-.34zm0-3.354V6h-.646a1.5 1.5 0 0 1 .646.646M16 8a1.5 1.5 0 0 1-1.5 1.5v-3A1.5 1.5 0 0 1 16 8"/>
            </svg>
          </h1>
          <p style="font-size: 24px; opacity: 0.7; margin-bottom: 70px;">
            Tribal Nations have many different options to get power for EV charging stations. There are organizations that help Tribal Nations get low cost and renewable energy that can be used for anything, including electric vehicles. One example of this would be <a href="https://www.ncai.org/" target="_blank">NCAI.org</a> which has worked with Tribal communities to integrate renewable energy and electric vehicles.
          </p>
        </div>
      </div>
    </div>

    <div class="geographic slide" style="background-color: white; height: 100vh">
      <div class="row">
        <div class="cell" style="width: 100%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 3.5vw; color: black;">
            Geographic Challenges
            <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" fill="currentColor" class="bi bi-geo" viewBox="0 0 16 16">
              <path fill-rule="evenodd" d="M8 1a3 3 0 1 0 0 6 3 3 0 0 0 0-6M4 4a4 4 0 1 1 4.5 3.969V13.5a.5.5 0 0 1-1 0V7.97A4 4 0 0 1 4 3.999zm2.493 8.574a.5.5 0 0 1-.411.575c-.712.118-1.28.295-1.655.493a1.3 1.3 0 0 0-.37.265.3.3 0 0 0-.057.09V14l.002.008.016.033a.6.6 0 0 0 .145.15c.165.13.435.27.813.395.751.25 1.82.414 3.024.414s2.273-.163 3.024-.414c.378-.126.648-.265.813-.395a.6.6 0 0 0 .146-.15l.015-.033L12 14v-.004a.3.3 0 0 0-.057-.09 1.3 1.3 0 0 0-.37-.264c-.376-.198-.943-.375-1.655-.493a.5.5 0 1 1 .164-.986c.77.127 1.452.328 1.957.594C12.5 13 13 13.4 13 14c0 .426-.26.752-.544.977-.29.228-.68.413-1.116.558-.878.293-2.059.465-3.34.465s-2.462-.172-3.34-.465c-.436-.145-.826-.33-1.116-.558C3.26 14.752 3 14.426 3 14c0-.599.5-1 .961-1.243.505-.266 1.187-.467 1.957-.594a.5.5 0 0 1 .575.411"/>
            </svg>
          </h1>
          <p style="font-size: 24px; opacity: 0.7; margin-bottom: 70px;">
            Despite the state's network of 1,200 charging stations, only 29 are located in the Upper Peninsula (U.P.), leaving rural areas underserved and creating "charging deserts." This highlights a pressing need for greater charging access, particularly for local businesses and tribal communities. To facilitate this transition, it is crucial to provide resources and technical assistance to Tribal Nations, empowering them to adopt electric vehicles (EVs) and clean energy solutions. However, EV adoption in these regions faces significant challenges. Vast distances between cities and towns with little infrastructure make it difficult for tribal communities to potentially integrate EV technology. Additionally, cold weather reduces battery performance, slows charging times, and decreases driving range, all of which complicate the efficient operation of EVs during winter months.
          </p>
        </div>
      </div>
    </div>

    <div class="iniative slide" style="background-color: white; height: 100vh">
      <div class="row">
        <div class="cell" style="width: 100%; color: black; flex-direction: column;">
          <h1 style="margin-top: 70px; font-size: 2.5vw; color: black;">The Document National Electric Vehicle Initiative for Tribal Nations</h1>
          <p style="font-size: 20px; opacity: 0.7; margin-bottom: 70px;">
            The document National Electric Vehicle Initiative for Tribal Nations, published by Indian Affairs, outlines a federal initiative to support the adoption of electric vehicles and charging infrastructure within tribal communities across the United States. The initiative aims to reduce emissions, promote sustainable energy, and improve transportation access for tribal nations, aligning with environmental and economic development goals. It addresses funding sources, technical assistance, and partnerships between federal agencies and tribal governments, acknowledging the unique challenges these communities face, such as limited infrastructure and resources. This initiative represents a step toward equitable access to clean energy and sustainable transportation solutions in tribal areas.
          </p>
          <p style="font-size: 18px; opacity: 0.7; margin-bottom: 70px;">
            <strong>Explanation: </strong> The initiative helps with funding and kickstarting the deployment of EV infrastructure, when otherwise they face problems with funding and the planning of these stations. Tribal nations being able to implement the chargers helps them promote proactive climate change actions and take steps forward to a better climate. Another way this helps is it empowers these because they get to help build and plan these changes as well 
          </p>
        </div>
      </div>
    </div>

  </div>

</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      slides: [],
      currentSlideIndex: 0,
      canScroll: false,
      scrolled: 0,
    }
  },
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
    },

    /**
     * Scroll down to the problem page
     */
    goToProblemPage() {
      const problemSection = document.querySelector('.problem');
      problemSection.scrollIntoView({ behavior:'smooth' });
    },

    /**
     * Check if the first slide is in view
     */
    checkFirstSlideInView() {
      const firstSlide = document.querySelector('.problem');
      const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            this.canScroll = true;
            observer.disconnect();
          }
        });
      }, {
        threshold: 0.1 // Trigger when at least 10% of the slide is visible
      });

      observer.observe(firstSlide);
    },

    /**
     * Find the current slide based on scroll position
     */
    findCurrentSlide() {
      const viewportHeight = window.innerHeight;
      
      for (let i = 0; i < this.slides.length; i++) {
        const slide = this.slides[i];
        const rect = slide.getBoundingClientRect();
        
        // Check if the slide is more than 50% in view
        if (rect.top <= viewportHeight / 2 && rect.bottom >= viewportHeight / 2) {
          this.currentSlideIndex = i;
          break;
        }
      }
    },

    /**
     * Scroll to the next slide
     */
    scrollToNextSlide() {
      if (!this.canScroll) return;

      // Find the current slide first to ensure accuracy
      this.findCurrentSlide();

      // Increment to next slide
      let nextIndex = this.currentSlideIndex + 1;
      
      // Wrap around to first slide if at the end
      if (nextIndex >= this.slides.length) {
        nextIndex = 0;
      }

      // Scroll to the next slide
      this.slides[nextIndex].scrollIntoView({ 
        behavior: 'smooth' 
      });
    },

    /**
     * Set up scroll event listener
     */
    setupScrollTracking() {
      // Get all slides
      this.slides = Array.from(document.querySelectorAll('.slide'));

      // Debounce scroll event to improve performance
      let scrollTimeout;
      window.addEventListener('scroll', () => {
        clearTimeout(scrollTimeout);
        scrollTimeout = setTimeout(this.findCurrentSlide, 100);
      });
    }
  },
  mounted() {
    this.animateBlades();
    this.checkFirstSlideInView();
    this.setupScrollTracking();

    // Scroll event listener
      window.addEventListener('scroll', function() {
      const scrollPosition = window.scrollY;
      const documentHeight = document.documentElement.scrollHeight - window.innerHeight;
      const scrollPercentage = (scrollPosition / documentHeight) * 100;
      this.scrolled = scrollPercentage;
    }.bind(this));

    // Add event listener to the next button
    const nextButton = document.querySelector('.next');
    nextButton.addEventListener('click', this.scrollToNextSlide);
  },
  beforeUnmount() {
    // Clean up event listener
    const nextButton = document.querySelector('.next');
    nextButton.removeEventListener('click', this.scrollToNextSlide);
  }
}
</script>

<style scoped>
  .windmill {
    position: absolute;
    /* Scale up */
    transform: scale(1.8);
  }

  .next {
    position: fixed;
    bottom: 25px;
    z-index: 1000;
    left: 50%;
    width: 200px;
    transform: translateX(-50%);
    display: none !important;
  }
  .visible {
    display: block !important;
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
