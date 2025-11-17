<template>
  <div class="testimonial-section">
    <div class="customer-success">Customer Success</div>
    <h3 class="testimonial-header">Trusted by Leading <span>Fleet Operators</span></h3>
    <p class="testimonial-desc">See how companies across Kenya are transforming their fleet operations with SparQ Edge.</p>
     <div class="testimonials-container">
    <div 
      v-for="(testimonial, index) in testimonials" 
      :key="index" 
      class="testimonial"
    >
      <ul class="stars-container">
        <li v-for="star in 4" :key="star" class="stars">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="17" viewBox="0 0 16 17" fill="none">
            <path
              d="M7.68334 2.1236C7.71255 2.06457 7.75768 2.01489 7.81364 1.98015C7.86959 1.94541 7.93414 1.927 8 1.927C8.06586 1.927 8.13041 1.94541 8.18637 1.98015C8.24232 2.01489 8.28746 2.06457 8.31667 2.1236L9.85667 5.24293C9.95812 5.44824 10.1079 5.62587 10.2931 5.76057C10.4783 5.89526 10.6934 5.98301 10.92 6.01626L14.364 6.52026C14.4293 6.52972 14.4906 6.55725 14.541 6.59973C14.5914 6.64222 14.629 6.69796 14.6494 6.76067C14.6697 6.82337 14.6722 6.89054 14.6564 6.95456C14.6406 7.01858 14.6072 7.0769 14.56 7.12293L12.0693 9.54826C11.9051 9.70833 11.7822 9.90592 11.7112 10.124C11.6403 10.3421 11.6234 10.5742 11.662 10.8003L12.25 14.2269C12.2615 14.2922 12.2545 14.3593 12.2297 14.4207C12.2049 14.4821 12.1633 14.5353 12.1097 14.5743C12.0561 14.6132 11.9927 14.6363 11.9266 14.6409C11.8605 14.6455 11.7945 14.6314 11.736 14.6003L8.65734 12.9816C8.45448 12.8751 8.22879 12.8194 7.99967 12.8194C7.77055 12.8194 7.54486 12.8751 7.342 12.9816L4.264 14.6003C4.20556 14.6312 4.1396 14.6451 4.07364 14.6404C4.00767 14.6357 3.94435 14.6126 3.89087 14.5737C3.83739 14.5348 3.79589 14.4817 3.77111 14.4204C3.74632 14.3591 3.73924 14.2921 3.75067 14.2269L4.338 10.8009C4.3768 10.5748 4.35999 10.3425 4.28903 10.1243C4.21807 9.90606 4.09508 9.70837 3.93067 9.54826L1.44 7.1236C1.3924 7.07762 1.35867 7.0192 1.34265 6.95498C1.32663 6.89077 1.32896 6.82334 1.34939 6.76039C1.36982 6.69744 1.40752 6.64149 1.45819 6.59892C1.50886 6.55635 1.57047 6.52886 1.636 6.5196L5.07934 6.01626C5.30618 5.98326 5.5216 5.89564 5.70706 5.76092C5.89252 5.62621 6.04247 5.44845 6.144 5.24293L7.68334 2.1236Z"
              fill="#FDC700"
              stroke="#FDC700"
              stroke-width="1.33333"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </li>
      </ul>
      
      <div class="quote">
        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="33" viewBox="0 0 32 33" fill="none">
          <path
            d="M21.3333 4.59375C20.6261 4.59375 19.9478 4.8747 19.4477 5.3748C18.9476 5.8749 18.6667 6.55317 18.6667 7.26042V15.2604C18.6667 15.9677 18.9476 16.6459 19.4477 17.146C19.9478 17.6461 20.6261 17.9271 21.3333 17.9271C21.687 17.9271 22.0261 18.0676 22.2761 18.3176C22.5262 18.5677 22.6667 18.9068 22.6667 19.2604V20.5938C22.6667 21.301 22.3857 21.9793 21.8856 22.4794C21.3855 22.9795 20.7072 23.2604 20 23.2604C19.6464 23.2604 19.3072 23.4009 19.0572 23.6509C18.8071 23.901 18.6667 24.2401 18.6667 24.5938V27.2604C18.6667 27.614 18.8071 27.9532 19.0572 28.2032C19.3072 28.4533 19.6464 28.5938 20 28.5938C22.1217 28.5938 24.1566 27.7509 25.6569 26.2506C27.1572 24.7503 28 22.7155 28 20.5938V7.26042C28 6.55317 27.7191 5.8749 27.219 5.3748C26.7189 4.8747 26.0406 4.59375 25.3333 4.59375H21.3333Z"
            stroke="#FF4D1E"
            stroke-width="2.66667"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M6.66667 4.59375C5.95942 4.59375 5.28115 4.8747 4.78105 5.3748C4.28095 5.8749 4 6.55317 4 7.26042V15.2604C4 15.9677 4.28095 16.6459 4.78105 17.146C5.28115 17.6461 5.95942 17.9271 6.66667 17.9271C7.02029 17.9271 7.35943 18.0676 7.60948 18.3176C7.85952 18.5677 8 18.9068 8 19.2604V20.5938C8 21.301 7.71905 21.9793 7.21895 22.4794C6.71885 22.9795 6.04058 23.2604 5.33333 23.2604C4.97971 23.2604 4.64057 23.4009 4.39052 23.6509C4.14048 23.901 4 24.2401 4 24.5938V27.2604C4 27.614 4.14048 27.9532 4.39052 28.2032C4.64057 28.4533 4.97971 28.5938 5.33333 28.5938C7.45507 28.5938 9.4899 27.7509 10.9902 26.2506C12.4905 24.7503 13.3333 22.7155 13.3333 20.5938V7.26042C13.3333 6.55317 13.0524 5.8749 12.5523 5.3748C12.0522 4.8747 11.3739 4.59375 10.6667 4.59375H6.66667Z"
            stroke="#FF4D1E"
            stroke-width="2.66667"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
      
      <p class="customer-testimonial">{{ testimonial.text }}</p>
      
      <div class="customer">
        <img :src="testimonial.image" :alt="testimonial.name" class="customer-img" />
        <div class="customer-details">
          <p class="customer-name">{{ testimonial.name }}</p>
          <p class="customer-position">{{ testimonial.position }}</p>
          <p class="customer-company">{{ testimonial.company }}</p>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>

<script setup>
const testimonials = [
  {
    text: '"SparQ Edge reduced our fuel costs by 30% and improved driver safety significantly. The platform is a game-changer."',
    image: '/images/no_img.webp',
    name: 'David Kimani',
    position: 'Fleet Manager',
    company: 'Urban Delivery Services'
  },
  {
    text: '"Your testimonial text here for the second customer."',
    image: '/images/no_img.webp',
    name: 'Jane Doe',
    position: 'Operations Director',
    company: 'Logistics Pro'
  },
  {
    text: '"Your testimonial text here for the third customer."',
    image: '/images/no_img.webp',
    name: 'John Smith',
    position: 'CEO',
    company: 'Transport Solutions'
  }
]
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@media (min-width: 1440px) {
  .testimonials-container {
  display: flex;
  flex-direction: row !important;
  flex-wrap: wrap;
}

.testimonial-section {
  padding: 8rem 8rem 10rem 8rem !important;
}

.testimonial {
width: calc((100% - 3rem) / 3) !important;
}
}

.testimonial-section {
  padding: 8rem 2rem 10rem 2rem;
  background-color: #fff;
}

.customer-success {
  color: #ff4d1e;
  /* font-family: Arimo; */
  font-size: 0.875rem;
  font-style: normal;
  font-weight: 600;
  line-height: 1.25rem; /* 142.857% */
  border-radius: 2097150rem;
  background: rgba(255, 77, 30, 0.2);
  width: fit-content;
  padding: 0.4rem 1rem;
  margin: auto;
}

.testimonial-header {
  color: #101828;
  text-align: center;
  /* font-family: Arimo; */
  font-size: 2.25rem;
  font-style: normal;
  font-weight: 700;
  line-height: 2.5rem; /* 111.111% */
  margin-top: 1.5rem;
  span {
    color: #ff4d1e;
  }
}

.testimonial-desc {
  color: #4a5565;
  text-align: center;
  /* font-family: Arimo; */
  font-size: 1.25rem;
  font-style: normal;
  font-weight: 400;
  line-height: 1.75rem; /* 140% */
}

.testimonials-container {
  margin-top: 1.5rem;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.testimonial {
  border-radius: 0.875rem;
  border: 1px solid rgba(0, 0, 0, 0.1);
  background: #fff;
  padding: 2rem;
  width: 100%;
 
  height: 22rem;
}

.stars-container {
  display: flex;
  gap: 1rem;
  margin-bottom: 2rem;
}

.quote {
  margin-bottom: 2rem;
}

.customer {
  margin-top: 1.5rem;
  display: flex;
  gap: 1rem;
  align-items: center;
}

.customer-img {
  height: 3rem;
  width: 3rem;
  border-radius: 50%;
}

.customer-details {
  display: flex;
  flex-direction: column;
  gap: 0.1rem;
}

.customer-name {
  color: #101828;
  font-size: 1rem;
  font-style: normal;
  font-weight: 700;
  line-height: 1.5rem; /* 150% */
}

.customer-position {
  color: #4a5565;
  font-size: 0.875rem;
  font-style: normal;
  font-weight: 400;
  line-height: 1.25rem; /* 142.857% */
}

.customer-company {
  color: #ff4d1e;
  font-size: 0.875rem;
  font-style: normal;
  font-weight: 400;
  line-height: 1.25rem; /* 142.857% */
}
</style>
