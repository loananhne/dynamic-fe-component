<template>
  <section id="why-us" class="why-us section-bg">
    <div class="container" data-aos="fade-up">
      <div class="row gy-4">
        <div class="col-lg-4" data-aos="fade-up" data-aos-delay="100">
          <div class="why-box">
            <h3>Why Choose Yummy?</h3>
            <p>
              Our restaurant focuses on creating customer satisfaction in terms
              of food quality and service for customers to experience.
            </p>
            <div class="text-center">
              <a href="#" class="more-btn"
                >Learn More <i class="bx bx-chevron-right"></i
              ></a>
            </div>
          </div>
        </div>

        <div class="col-lg-8 d-flex align-items-center">
          <div class="row gy-4">
            <div class="col-xl-4" data-aos="fade-up" data-aos-delay="200">
              <div
                class="icon-box d-flex flex-column justify-content-center align-items-center"
              >
                <h4>Food quality</h4>
                <p>
                  From the best food sources, we bring great dishes prepared by
                  talented and famous chefs.Focus on ensuring hygiene and food
                  safety, providing nutritious and healthy dishes.
                </p>
              </div>
            </div>

            <div class="col-xl-4" data-aos="fade-up" data-aos-delay="300">
              <div
                class="icon-box d-flex flex-column justify-content-center align-items-center"
              >
                <h4>Luxury space</h4>
                <p>
                  We want customers to be able to enjoy great food in a
                  luxurious, comfortable space.
                </p>
              </div>
            </div>

            <div class="col-xl-4" data-aos="fade-up" data-aos-delay="400">
              <div
                class="icon-box d-flex flex-column justify-content-center align-items-center"
              >
                <h4>Luxury space</h4>
                <p>
                  Bringing customer satisfaction with the service experience
                  here is one of our important things, attentive service staff
                  as well as many incentives for customers.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script></script>
<style scoped>
.why-us .why-box {
  padding: 30px;
  background: var(--color-primary);
  color: #fff;
}

.why-us .why-box h3 {
  font-weight: 700;
  font-size: 34px;
  margin-bottom: 30px;
}

.why-us .why-box p {
  margin-bottom: 30px;
}

.why-us .why-box .more-btn {
  display: inline-block;
  background: rgba(255, 255, 255, 0.3);
  padding: 6px 30px 8px 30px;
  color: #fff;
  border-radius: 50px;
  transition: all ease-in-out 0.4s;
}

.why-us .why-box .more-btn i {
  font-size: 14px;
}

.why-us .why-box .more-btn:hover {
  color: var(--color-primary);
  background: #fff;
}

.why-us .icon-box {
  text-align: center;
  background: #fff;
  padding: 40px 30px;
  width: 100%;
  height: 100%;
  border: 1px solid rgba(55, 55, 63, 0.1);
  transition: 0.3s;
}

.why-us .icon-box i {
  color: var(--color-primary);
  margin-bottom: 30px;
  font-size: 32px;
  margin-bottom: 30px;
  background: rgba(206, 18, 18, 0.1);
  border-radius: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 64px;
  height: 64px;
}

.why-us .icon-box h4 {
  font-size: 20px;
  font-weight: 400;
  margin: 0 0 30px 0;
  font-family: var(--font-secondary);
}

.why-us .icon-box p {
  font-size: 15px;
  color: #6c757d;
}

@media (min-width: 1200px) {
  .why-us .icon-box:hover {
    transform: scale(1.1);
  }
}
</style>
