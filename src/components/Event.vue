<template>
  <section id="events" class="events">
    <div class="container-fluid" data-aos="fade-up">
      <div class="section-header">
        <h2>Events</h2>
        <p>Share <span>Your Moments</span> In Our Restaurant</p>
      </div>

      <div class="slides-3 swiper" data-aos="fade-up" data-aos-delay="100">
        <div class="swiper-wrapper">
          <div
            class="swiper-slide event-item d-flex flex-column justify-content-end"
            style="background-image: url(../assets/img/events-1.jpg)"
          >
          <img src="../assets/img/hero-img.png" class="img-fluid" alt="" data-aos="zoom-out" data-aos-delay="300">
            <h3>Custom Parties</h3>
            <div class="price align-self-start">$99</div>
            <p class="description">
              Quo corporis voluptas ea ad. Consectetur inventore sapiente ipsum
              voluptas eos omnis facere. Enim facilis veritatis id est rem
              repudiandae nulla expedita quas.
            </p>
          </div>

          <div
            class="swiper-slide event-item d-flex flex-column justify-content-end"
            style="background-image: url(../assets/img/events-2.jpg)"
          >
            <h3>Private Parties</h3>
            <div class="price align-self-start">$289</div>
            <p class="description">
              In delectus sint qui et enim. Et ab repudiandae inventore quaerat
              doloribus. Facere nemo vero est ut dolores ea assumenda et.
              Delectus saepe accusamus aspernatur.
            </p>
          </div>

          <div
            class="swiper-slide event-item d-flex flex-column justify-content-end"
            style="background-image: url(../assets/img/events-3.jpg)"
          >
          
            <h3>Birthday Parties</h3>
            <div class="price align-self-start">$499</div>
            <p class="description">
              Laborum aperiam atque omnis minus omnis est qui assumenda quos.
              Quis id sit quibusdam. Esse quisquam ducimus officia ipsum ut
              quibusdam maxime. Non enim perspiciatis.
            </p>
          </div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.events .container-fluid {
  padding: 0;
}

.events .event-item {
  background-size: cover;
  background-position: cente;
  min-height: 600px;
  padding: 30px;
}

@media (max-width: 575px) {
  .events .event-item {
    min-height: 500px;
  }
}

.events .event-item:before {
  content: "";
  background: rgba(0, 0, 0, 0.6);
  position: absolute;
  inset: 0;
}

.events .event-item h3 {
  font-size: 24px;
  font-weight: 700;
  margin-bottom: 5px;
  color: #fff;
  position: relative;
}

.events .event-item .price {
  color: #fff;
  border-bottom: 2px solid var(--color-primary);
  font-size: 32px;
  font-weight: 700;
  margin-bottom: 15px;
  position: relative;
}

.events .event-item .description {
  margin-bottom: 0;
  color: rgba(255, 255, 255, 0.9);
  position: relative;
}

@media (min-width: 1200px) {
  .events .swiper-slide-active+.swiper-slide {
    border-left: 1px solid rgba(255, 255, 255, 0.5);
    border-right: 1px solid rgba(255, 255, 255, 0.5);
    z-index: 1;
  }
}

.events .swiper-pagination {
  margin-top: 20px;
  position: relative;
}

.events .swiper-pagination .swiper-pagination-bullet {
  width: 10px;
  height: 10px;
  background-color: #d1d1d7;
  opacity: 1;
}

.events .swiper-pagination .swiper-pagination-bullet-active {
  background-color: var(--color-primary);
}
</style>
