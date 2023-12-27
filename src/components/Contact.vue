<script></script>

<template>
  <section id="contact" class="contact">
    <div class="container" data-aos="fade-up">
      <div class="section-header">
        <h2>Contact</h2>
        <p>Need Help? <span>Contact Us</span></p>
      </div>

      <div class="mb-3">
        <iframe
          style="border: 0; width: 100%; height: 350px"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3928.973205297408!2d105.75759637479388!3d10.019069690087298!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31a088482fb773f7%3A0x6b3fac9bccaf9430!2zSOG6u20gMTMyIMSQLiAzIFRow6FuZyAyLCBBbiBCaW5oLCBIxrBuZyBM4bujaSwgTmluaCBLaeG7gXUsIEPhuqduIFRoxqEsIFZp4buHdCBOYW0!5e0!3m2!1svi!2s!4v1703651932945!5m2!1svi!2s"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </div>

      <div class="row gy-4">
        <div class="col-md-6">
          <div class="info-item d-flex align-items-center">
            <div>
              <h3>Our Address</h3>
              <p>132, 3/2 Street, Ninh Kieu, Can Tho</p>
            </div>
          </div>
        </div>

        <div class="col-md-6">
          <div class="info-item d-flex align-items-center">
            <div>
              <h3>Email Us</h3>
              <p>contact@example.com</p>
            </div>
          </div>
        </div>

        <div class="col-md-6">
          <div class="info-item d-flex align-items-center">
            <div>
              <h3>Call Us</h3>
              <p>+0889 930 738</p>
            </div>
          </div>
        </div>

        <div class="col-md-6">
          <div class="info-item d-flex align-items-center">
            <div>
              <h3>Opening Hours</h3>
              <div>
                <strong>Mon-Sat:</strong> 11AM - 23PM;
                <strong>Sunday:</strong> Closed
              </div>
            </div>
          </div>
        </div>
      </div>

      <form
        action="forms/contact.php"
        method="post"
        role="form"
        class="php-email-form p-3 p-md-4"
      >
        <div class="row">
          <div class="col-xl-6 form-group">
            <input
              type="text"
              name="name"
              class="form-control"
              id="name"
              placeholder="Your Name"
              required
            />
          </div>
          <div class="col-xl-6 form-group">
            <input
              type="email"
              class="form-control"
              name="email"
              id="email"
              placeholder="Your Email"
              required
            />
          </div>
        </div>
        <div class="form-group">
          <input
            type="text"
            class="form-control"
            name="subject"
            id="subject"
            placeholder="Subject"
            required
          />
        </div>
        <div class="form-group">
          <textarea
            class="form-control"
            name="message"
            rows="5"
            placeholder="Message"
            required
          ></textarea>
        </div>
        <div class="my-3">
          <div class="loading">Loading</div>
          <div class="error-message"></div>
          <div class="sent-message">Your message has been sent. Thank you!</div>
        </div>
        <div class="text-center">
          <button type="submit">Send Message</button>
        </div>
      </form>
    </div>
  </section>
</template>

<style scoped>
.contact .info-item {
  background: #f4f4f4;
  padding: 30px;
  height: 100%;
}

.contact .info-item .icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 56px;
  height: 56px;
  font-size: 24px;
  line-height: 0;
  color: #fff;
  background: var(--color-primary);
  border-radius: 50%;
  margin-right: 15px;
}

.contact .info-item h3 {
  font-size: 20px;
  color: #6c757d;
  font-weight: 700;
  margin: 0 0 5px 0;
}

.contact .info-item p {
  padding: 0;
  margin: 0;
  line-height: 24px;
  font-size: 14px;
}

.contact .info-item .social-links a {
  font-size: 24px;
  display: inline-block;
  color: rgba(55, 55, 63, 0.7);
  line-height: 1;
  margin: 4px 6px 0 0;
  transition: 0.3s;
}

.contact .info-item .social-links a:hover {
  color: var(--color-primary);
}

.contact .php-email-form {
  width: 100%;
  margin-top: 30px;
  background: #fff;
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.08);
}

.contact .php-email-form .form-group {
  padding-bottom: 20px;
}

.contact .php-email-form .error-message {
  display: none;
  color: #fff;
  background: #df1529;
  text-align: left;
  padding: 15px;
  font-weight: 600;
}

.contact .php-email-form .error-message br + br {
  margin-top: 25px;
}

.contact .php-email-form .sent-message {
  display: none;
  color: #fff;
  background: #059652;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}

.contact .php-email-form .loading {
  display: none;
  background: #fff;
  text-align: center;
  padding: 15px;
}

.contact .php-email-form .loading:before {
  content: "";
  display: inline-block;
  border-radius: 50%;
  width: 24px;
  height: 24px;
  margin: 0 10px -6px 0;
  border: 3px solid #059652;
  border-top-color: #fff;
  animation: animate-loading 1s linear infinite;
}

.contact .php-email-form input,
.contact .php-email-form textarea {
  border-radius: 0;
  box-shadow: none;
  font-size: 14px;
}

.contact .php-email-form input:focus,
.contact .php-email-form textarea:focus {
  border-color: var(--color-primary);
}

.contact .php-email-form input {
  height: 48px;
}

.contact .php-email-form textarea {
  padding: 10px 12px;
}

.contact .php-email-form button[type="submit"] {
  background: var(--color-primary);
  border: 0;
  padding: 12px 40px;
  color: #fff;
  transition: 0.4s;
  border-radius: 50px;
}

.contact .php-email-form button[type="submit"]:hover {
  background: #ec2727;
}

@keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}
</style>
