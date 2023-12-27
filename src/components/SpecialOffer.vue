<script></script>

<template>
  <div class="special-offer">
    <v-container class="special-offer__frame">
      <v-row>
        <v-col cols="3" class="special-offer__frame--left">
          <div class="special-offer__menu">
            <p class="special-offer--title">special-offer</p>
            <p class="special-offer--detail">
              When you buy three cakes of ... of two cakes you buy three cakes
              of ... of two cakes you buy three cakes of ... of two cakes you
              buy three cakes of
            </p>
            <a href="#" class="order-button">To Order</a>
          </div>
        </v-col>
        <v-col cols="9" class="special-offer__frame--right">
          <img src="../assets/pictures/cake2.jpg" class="img-fluid" alt="..." />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style scoped>
.special-offer {
  height: 100vh;
  /* display: flex; */
  justify-content: center;
  align-items: center;
  margin: 0;
  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  color: #ffff;
  background-color: #e9eaea;
}

.special-offer__frame--left {
  background-color: #9f0311;
}
.special-offer__frame--right {
  margin-top: -13px;
}

@media (min-width: 600px) and (max-width: 900px) {
  .v-col {
    flex-basis: 50%;
    max-width: 50%;
  }
}

@media (max-width: 900px) {
  .v-col {
    flex-basis: 100%;
    max-width: 100%;
  }
  .special-offer__frame--left,
  .special-offer__frame--right {
    padding: 10px;
  }
  .special-offer__menu {
    border-right: none;
    border-bottom: 5px solid #f05545;
  }
}
</style>
