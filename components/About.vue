<template>
  <div class="about-section">
    <div class="abt-container">
      <div class="abt-edge-badge">
        <p>About SparQ Edge</p>
      </div>
      <div class="abt-info-container">
        <div class="abt-desc">
          <h5 class="abt-heading">Built for Africa, <span>Powered by Innovation</span></h5>
          <p class="abt-text">We understand the unique challenges of fleet management in Africa. Our platform delivers
            world-class solutions designed for local conditions.</p>
          <ul class="feature-container">
            <li v-for="(feature, index) in features" :key="index" class="feature">
              <svg xmlns="http://www.w3.org/2000/svg" width="20" height="21" viewBox="0 0 20 21" fill="none">
                <path
                  d="M18.1675 8.92707C18.5481 10.7948 18.2769 12.7366 17.399 14.4286C16.5212 16.1205 15.0899 17.4604 13.3438 18.2248C11.5976 18.9892 9.6422 19.1319 7.80359 18.629C5.96498 18.1262 4.35433 17.0082 3.24024 15.4616C2.12614 13.9149 1.57594 12.0331 1.68139 10.1299C1.78684 8.22669 2.54157 6.41715 3.81972 5.00305C5.09786 3.58895 6.82216 2.65577 8.70506 2.35912C10.588 2.06247 12.5157 2.42029 14.1667 3.37291"
                  stroke="#FF4D1E" stroke-width="1.66667" stroke-linecap="round" stroke-linejoin="round" />
                <path d="M7.5 9.76034L10 12.2603L18.3333 3.927" stroke="#FF4D1E" stroke-width="1.66667"
                  stroke-linecap="round" stroke-linejoin="round" />
              </svg>
              <p>{{ feature }}</p>
            </li>
          </ul>
          <div class="abt-btns">
            <button class="learn-btn">Learn More</button>
            <button class="abt-contact">Contact Us</button>
          </div>
        </div>
        <div class="abt-img">
          <img src="/images/high-five.jpg" alt="" class="abt-image" />
          <div class="founded">
            <p class="year">2024</p>
            <p class="location">Founded in Nairobi</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const features = ["Easy Excel upload (CSV/XLS/XLSX) with instant validation", "Auto-generated dashboards and charts for quick insights", "Dive deeper with interactive analysis and one-click reports", "Compliance with local regulations"];
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


@media (min-width: 1440px) {
  .abt-container {
    padding-bottom: 1rem !important;
  }

  .about-section {
    padding-left: 8rem !important;
    padding-right: 8rem !important;
  }

  .abt-info-container {
    display: flex;
    flex-direction: row !important;
    gap: 3rem;
  }

  .abt-desc {
    margin-bottom: 0rem;
  }

  .abt-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .abt-image {
    border-radius: 1rem;
    width: 100%;
  }

  .abt-text {
    margin-bottom: 4rem !important;
  }

  .abt-btns {
    display: flex;
    flex-direction: row !important;
    gap: 1rem;
    margin-top: 2rem !important;
  }

  .learn-btn {
    padding: 0.8rem 1.5rem !important;
  }

  .abt-contact {
    padding: 0.8rem 1.5rem !important;
  }
}

.about-section {
  background: white;
  padding-left: 2rem;
  padding-right: 2rem;
}

.abt-container {
  padding: 2rem 2rem 8rem 2rem;
  background: #f9fafb;
  display: flex;
  flex-direction: column;
}

.abt-info-container {
  display: flex;
  flex-direction: column;
}

.abt-edge-badge {
  color: #ff4d1e;
  /* font-family: Arimo; */
  font-size: 0.875rem;
  font-style: normal;
  font-weight: 600;
  line-height: 1.25rem;
  /* 142.857% */
  border-radius: 2097150rem;
  background: rgba(255, 77, 30, 0.2);
  width: fit-content;
  padding: 0.4rem 1rem;
  margin-bottom: 1.5rem;
}

.abt-desc {
  margin-bottom: 3rem;
}

.abt-heading {
  color: #101828;
  /* font-family: Arimo; */
  font-size: 2rem;
  font-style: normal;
  font-weight: 700;
  line-height: 2.5rem;
  /* 125% */
  margin-bottom: 1.5rem;

  span {
    color: #ff4d1e;
  }
}

.abt-text {
  color: #4a5565;
  /* font-family: Arimo; */
  font-size: 1.25rem;
  font-style: normal;
  font-weight: 400;
  line-height: 1.75rem;
  /* 140% */
  margin-bottom: 1.5rem;
}

.feature {
  display: flex;
  align-items: center;
  gap: 1rem;
  color: #364153;
  /* font-family: Arimo; */
  font-size: 1rem;
  font-style: normal;
  font-weight: 400;
  line-height: 1.5rem;
  /* 150% */
  margin-bottom: 0.8rem;
}

.abt-btns {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  margin-top: 2rem;
}

.learn-btn {
  padding: 1rem;
  border-radius: 0.5rem;
  border-radius: 0.5rem;
  background: #ff4d1e;
  color: #fff;
  /* font-family: Arimo; */
  font-size: 1.125rem;
  font-style: normal;
  font-weight: 600;
  line-height: 1.75rem;
  /* 155.556% */
}

.abt-contact {
  border-radius: 0.5rem;
  border: 1px solid #d1d5dc;
  background: #fff;
  padding: 1rem;
  font-size: 1.125rem;
  font-style: normal;
  font-weight: 600;
  line-height: 1.75rem;
}

.abt-img {
  position: relative;
  border-radius: 1rem;
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.1);
}

.founded {
  position: absolute;
  bottom: -2rem;
  left: -1rem;
  background: #fff;
  border-radius: 0.5rem;
  padding: 1.2rem 1rem;
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.1);

  .year {
    color: #ff4d1e;
    font-size: 1.5rem;
    font-style: normal;
    font-weight: 700;
    line-height: 2rem;
    /* 133.333% */
  }

  .location {
    color: #4a5565;
    font-size: 0.875rem;
    font-style: normal;
    font-weight: 400;
    line-height: 1.25rem;
    /* 142.857% */
  }
}
</style>
