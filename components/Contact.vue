<template>
  <section id="contact">
    <b-container>
      <h2>CONTACTO</h2>
      <b-row>
        <!--  -->
        <b-col class="contact" xs="12" sm="6" md="12" lg="4">
          <img src="../assets/icons/pin.svg" alt="location" />
          <h5>Localización</h5>
          <p>{{ location }}</p>
        </b-col>
        <!--  -->
        <b-col class="contact" xs="12" sm="6" md="12" lg="4">
          <img src="../assets/icons/linkedin.svg" alt="linkedin" />
          <h5>Linkedin</h5>
          <a href="https://www.linkedin.com/in/ángel-robles-0b309b80/">{{
            name
          }}</a>
        </b-col>
        <!--  -->
        <b-col class="contact" xs="12" sm="6" md="12" lg="4">
          <img src="../assets/icons/email.svg" alt="email" />
          <h5>E-mail</h5>
          <p>{{ mail }}</p>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
export default {
  data: () => ({
    name: "Angel Robles",
    location: "Chihuahua, Chi.",
    mail: "geloo.rb@gmail.com",
  }),
};
</script>

<style scoped>
#contact {
  background-color: #1a1a1a;
  align-items: center;
  padding: 40px 20px;
}

.contact {
  padding: 10px;
}

#contact h2 {
  font-weight: bold;
  font-size: 33px;
  color: #fff;
  margin-top: 15px;
  margin-bottom: 50px;
  letter-spacing: 4px;
}

#contact img {
  filter: invert(39%) sepia(87%) saturate(709%) hue-rotate(310deg)
    brightness(82%) contrast(105%);
  height: 40px;
  margin-bottom: 10px;
}

#contact h5 {
  color: #fff;
  font-weight: bold;
  font-size: 20px;
}

#contact p {
  color: #fff;
  font-size: 16px;
}

#contact a {
  color: #fff;
  font-size: 16px;
}

#contact .whatsapp {
  color: #075e54;
  font-size: 20px;
}
</style>
