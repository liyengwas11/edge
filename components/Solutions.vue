<template>
  <div class="solutions-section">
    <div class="soln-header">
      <h3>Complete Fleet Management <span>Solutions</span></h3>
      <p>Everything you need to manage, monitor, and optimize your fleet operations in one integrated platform.</p>
    </div>
    <div class="soln-cards-container">
      <div v-for="card in solutionCards" :key="card.id" class="soln-card">
        <div class="soln-icon">
          <div v-html="card.svg"></div>
        </div>
        <h5>{{ card.title }}</h5>
        <p>{{ card.description }}</p>
      </div>
    </div>
    <div class="optimize">
      <div class="optimize-header">
        <h3>Ready to Optimize Your Fleet?</h3>
        <p>Join hundreds of companies using SparQ Edge to reduce costs and improve efficiency.</p>
      </div>
      <div class="optimize-cta">
        <a href="" class="start-trial">Start Free Trial</a>
        <button class="demo">Request Demo</button>
      </div>
    </div>
    <div class="fleet-dashboard">
        <img src="/images/edge.png" class="dashboard-disp" alt="">
        <p class="dashboard-desc">Access Your Fleet Dashboard</p>
    </div>
  </div>
</template>

<script setup>
const solutionCards = [
  {
    id: 1,
    svg: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="25" viewBox="0 0 24 25" fill="none">
  <path d="M14 18.5938V6.59375C14 6.06332 13.7893 5.55461 13.4142 5.17954C13.0391 4.80446 12.5304 4.59375 12 4.59375H4C3.46957 4.59375 2.96086 4.80446 2.58579 5.17954C2.21071 5.55461 2 6.06332 2 6.59375V17.5938C2 17.859 2.10536 18.1133 2.29289 18.3009C2.48043 18.4884 2.73478 18.5938 3 18.5938H5" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M15 18.5938H9" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M19 18.5938H21C21.2652 18.5938 21.5196 18.4884 21.7071 18.3009C21.8946 18.1133 22 17.859 22 17.5938V13.9438C21.9996 13.7168 21.922 13.4968 21.78 13.3197L18.3 8.96975C18.2065 8.85263 18.0878 8.75803 17.9528 8.69295C17.8178 8.62787 17.6699 8.59396 17.52 8.59375H14" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M17 20.5938C18.1046 20.5938 19 19.6983 19 18.5938C19 17.4892 18.1046 16.5938 17 16.5938C15.8954 16.5938 15 17.4892 15 18.5938C15 19.6983 15.8954 20.5938 17 20.5938Z" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M7 20.5938C8.10457 20.5938 9 19.6983 9 18.5938C9 17.4892 8.10457 16.5938 7 16.5938C5.89543 16.5938 5 17.4892 5 18.5938C5 19.6983 5.89543 20.5938 7 20.5938Z" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>`,
    title: "Vehicle Management",
    description: "Real-time tracking, maintenance scheduling, and performance monitoring for your entire fleet.",
  },
  {
    id: 2,
    svg: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="25" viewBox="0 0 24 25" fill="none">
  <path d="M16 21.5938V19.5938C16 18.5329 15.5786 17.5155 14.8284 16.7653C14.0783 16.0152 13.0609 15.5938 12 15.5938H6C4.93913 15.5938 3.92172 16.0152 3.17157 16.7653C2.42143 17.5155 2 18.5329 2 19.5938V21.5938" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M16 3.7218C16.8578 3.94417 17.6174 4.44507 18.1597 5.14586C18.702 5.84666 18.9962 6.70769 18.9962 7.5938C18.9962 8.47991 18.702 9.34094 18.1597 10.0417C17.6174 10.7425 16.8578 11.2434 16 11.4658" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M22 21.5938V19.5938C21.9993 18.7075 21.7044 17.8465 21.1614 17.1461C20.6184 16.4456 19.8581 15.9453 19 15.7238" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M9 11.5938C11.2091 11.5938 13 9.80289 13 7.59375C13 5.38461 11.2091 3.59375 9 3.59375C6.79086 3.59375 5 5.38461 5 7.59375C5 9.80289 6.79086 11.5938 9 11.5938Z" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>`,
    title: "Driver Management",
    description: "Monitor driver behavior, safety metrics, and performance with comprehensive analytics.",
  },
  {
    id: 3,
    svg: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="25" viewBox="0 0 24 25" fill="none">
  <path d="M14 13.5938H16C16.5304 13.5938 17.0391 13.8045 17.4142 14.1795C17.7893 14.5546 18 15.0633 18 15.5938V17.5938C18 18.1242 18.2107 18.6329 18.5858 19.008C18.9609 19.383 19.4696 19.5938 20 19.5938C20.5304 19.5938 21.0391 19.383 21.4142 19.008C21.7893 18.6329 22 18.1242 22 17.5938V10.5957C22.0002 10.3318 21.9482 10.0705 21.8469 9.82678C21.7457 9.58307 21.5972 9.36181 21.41 9.17575L18 5.59375" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M14 21.5938V5.59375C14 5.06332 13.7893 4.55461 13.4142 4.17954C13.0391 3.80446 12.5304 3.59375 12 3.59375H5C4.46957 3.59375 3.96086 3.80446 3.58579 4.17954C3.21071 4.55461 3 5.06332 3 5.59375V21.5938" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M2 21.5938H15" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M3 9.59375H14" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>`,
    title: "Fuel Management",
    description: "Track consumption, prevent theft, and optimize fuel costs across all vehicles.",
  },
  {
    id: 4,
    svg: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="25" viewBox="0 0 24 25" fill="none">
  <path d="M3 3.59375V19.5938C3 20.1242 3.21071 20.6329 3.58579 21.008C3.96086 21.383 4.46957 21.5938 5 21.5938H21" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M18 17.5938V9.59375" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M13 17.5938V5.59375" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M8 17.5938V14.5938" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>`,
    title: "Aanalytics & Reporting",
    description: "Data-driven insights with customizable dashboards and automated reporting.",
  },
  {
    id: 5,
    svg: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="25" viewBox="0 0 24 25" fill="none">
  <path d="M20 13.5937C20 18.5937 16.5 21.0937 12.34 22.5437C12.1222 22.6175 11.8855 22.614 11.67 22.5337C7.5 21.0937 4 18.5937 4 13.5937V6.59371C4 6.32849 4.10536 6.07414 4.29289 5.8866C4.48043 5.69907 4.73478 5.59371 5 5.59371C7 5.59371 9.5 4.39371 11.24 2.87371C11.4519 2.69271 11.7214 2.59326 12 2.59326C12.2786 2.59326 12.5481 2.69271 12.76 2.87371C14.51 4.40371 17 5.59371 19 5.59371C19.2652 5.59371 19.5196 5.69907 19.7071 5.8866C19.8946 6.07414 20 6.32849 20 6.59371V13.5937Z" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>`,
    title: "Saftey & Compliance",
    description: "Ensure regulatory compliance and maintain safety standards across operations.",
  },
  {
    id: 6,
    svg: `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="25" viewBox="0 0 24 25" fill="none">
  <path d="M9.671 4.72978C9.7261 4.15012 9.99533 3.61182 10.4261 3.22006C10.8569 2.82829 11.4182 2.61121 12.0005 2.61121C12.5828 2.61121 13.1441 2.82829 13.5749 3.22006C14.0057 3.61182 14.2749 4.15012 14.33 4.72978C14.3631 5.10423 14.486 5.4652 14.6881 5.78212C14.8903 6.09904 15.1659 6.36259 15.4915 6.55046C15.8171 6.73832 16.1831 6.84498 16.5587 6.8614C16.9343 6.87782 17.3082 6.80352 17.649 6.64478C18.1781 6.40456 18.7777 6.3698 19.331 6.54727C19.8843 6.72473 20.3518 7.10173 20.6425 7.60488C20.9332 8.10804 21.0263 8.70135 20.9036 9.26935C20.781 9.83735 20.4514 10.3394 19.979 10.6778C19.6714 10.8936 19.4203 11.1804 19.2469 11.5138C19.0736 11.8472 18.983 12.2175 18.983 12.5933C18.983 12.9691 19.0736 13.3393 19.2469 13.6728C19.4203 14.0062 19.6714 14.2929 19.979 14.5088C20.4514 14.8472 20.781 15.3492 20.9036 15.9172C21.0263 16.4852 20.9332 17.0785 20.6425 17.5817C20.3518 18.0848 19.8843 18.4618 19.331 18.6393C18.7777 18.8168 18.1781 18.782 17.649 18.5418C17.3082 18.383 16.9343 18.3087 16.5587 18.3252C16.1831 18.3416 15.8171 18.4482 15.4915 18.6361C15.1659 18.824 14.8903 19.0875 14.6881 19.4044C14.486 19.7214 14.3631 20.0823 14.33 20.4568C14.2749 21.0364 14.0057 21.5747 13.5749 21.9665C13.1441 22.3583 12.5828 22.5754 12.0005 22.5754C11.4182 22.5754 10.8569 22.3583 10.4261 21.9665C9.99533 21.5747 9.7261 21.0364 9.671 20.4568C9.63794 20.0822 9.5151 19.7211 9.31286 19.4041C9.11063 19.087 8.83497 18.8234 8.50923 18.6355C8.18349 18.4476 7.81727 18.341 7.44158 18.3247C7.06589 18.3084 6.6918 18.3828 6.351 18.5418C5.82189 18.782 5.22233 18.8168 4.669 18.6393C4.11567 18.4618 3.64817 18.0848 3.35748 17.5817C3.06679 17.0785 2.97371 16.4852 3.09636 15.9172C3.219 15.3492 3.5486 14.8472 4.021 14.5088C4.32862 14.2929 4.57973 14.0062 4.75309 13.6728C4.92645 13.3393 5.01695 12.9691 5.01695 12.5933C5.01695 12.2175 4.92645 11.8472 4.75309 11.5138C4.57973 11.1804 4.32862 10.8936 4.021 10.6778C3.54926 10.3392 3.22025 9.83737 3.0979 9.26976C2.97555 8.70215 3.06861 8.10932 3.35898 7.60649C3.64936 7.10366 4.11631 6.72676 4.66909 6.54902C5.22187 6.37128 5.82098 6.40541 6.35 6.64478C6.69076 6.80352 7.06474 6.87782 7.4403 6.8614C7.81586 6.84498 8.18193 6.73832 8.50754 6.55046C8.83314 6.36259 9.10869 6.09904 9.31086 5.78212C9.51304 5.4652 9.63588 5.10423 9.669 4.72978" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M12 15.5938C13.6569 15.5938 15 14.2506 15 12.5938C15 10.9369 13.6569 9.59375 12 9.59375C10.3431 9.59375 9 10.9369 9 12.5938C9 14.2506 10.3431 15.5938 12 15.5938Z" stroke="#FF4D1E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>`,
    title: "System Management",
    description: "Configure sites, operators, and system settings with role-based access control.",
  },
];
</script>

<style scoped>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
@media (max-width: 1440px) {
  .fleet-dashboard {
    display: block;
  }
}

@media (min-width: 1440px) {
 .soln-cards-container {
    flex-direction: row !important;
    flex-wrap: wrap;
  }
  
  .soln-card {
    width: calc((100% - 4rem) / 3) !important; /* 3 cards with 2rem gap between them */
  }

  .solutions-section {
  padding: 8rem 8rem 10rem 8rem !important;
  background-color: #fff;
}

.fleet-dashboard {
  display: none;
}
}

.solutions-section {
  padding: 8rem 2rem 10rem 2rem;
  background-color: #fff;
}
.soln-header {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  margin-bottom: 4rem;

  h3 {
    color: #101828;
    text-align: center;
    /* font-family: Arimo; */
    font-size: 1.875rem;
    font-style: normal;
    font-weight: 700;
    line-height: 2.25rem;
    span {
      color: #ff4d1e;
    }
  }

  p {
    color: #4a5565;
    text-align: center;
    /* font-family: Arimo; */
    font-size: 1rem;
    font-style: normal;
    font-weight: 400;
    line-height: 1.5rem; /* 150% */
    max-width: 600px;
  }
}
.soln-cards-container {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.soln-card {
  border-radius: 0.875rem;
  border: 1px solid rgba(0, 0, 0, 0.1);
  background: #fff;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 3rem;
  padding: 2rem;
  width: 100%;
  h5 {
    color: #101828;
    font-size: 1.25rem;
    font-style: normal;
    font-weight: 700;
    line-height: 1.75rem;
  }
  p {
    color: #4a5565;
    font-size: 1rem;
    font-style: normal;
    font-weight: 400;
    line-height: 1.5rem; /* 150% */
  }
}

.soln-icon {
  padding: 1rem;
  border-radius: 0.625rem;
  background: rgba(255, 77, 30, 0.2);
  width: 3.8rem;
}

.optimize {
  margin-top: 5rem;
  border-radius: 1rem;
  background: #f9fafb;
  width: 100%;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 5rem;
}

.optimize-header {
  gap: 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;

  h3 {
    color: #101828;
    text-align: center;
    /* font-family: Arimo; */
    font-size: 1.875rem;
    font-style: normal;
    font-weight: 700;
    line-height: 2.25rem;
  }

  p {
    color: #4a5565;
    text-align: center;
    /* font-family: Arimo; */
    font-size: 1rem;
    font-style: normal;
    font-weight: 400;
    line-height: 1.5rem; /* 150% */
  }
}
.optimize-cta {
  margin-top: 2rem;
  display: flex;
  gap: 1rem;
  
}
.start-trial {
  border-radius: 0.5rem;
  background: #ff4d1e;
  color: #fff;
  padding: 0.7rem 1rem;
}

.demo {
  border-radius: 0.5rem;
  border: 1px solid #d1d5dc;
  background: #fff;
  padding: 0.7rem 1rem;
}

.fleet-dashboard {
    background: #F9FAFB;
    padding: 1rem;
}

.dashboard-desc {
  text-align: center;
  margin-top: 0.5rem;
  color: #6B7280;
  font-size: 1.5rem;
  font-style: normal;
  font-weight: 400;
  line-height: 1.5rem; /* 150% */
}

.dashboard-disp {
  width: 80%;
  height: auto;
  max-width: 1200px; /* Maximum width on large screens */
  display: block;
  margin: 0 auto; /* Center the image */
}

/* Tablet screens */
@media (max-width: 768px) {
  .dashboard-disp {
    max-width: 100%;
    padding: 0 20px; /* Add some spacing on sides */
  }
}

/* Mobile screens */
@media (max-width: 480px) {
  .dashboard-disp {
    max-width: 100%;
    padding: 0 10px;
  }
}
</style>
