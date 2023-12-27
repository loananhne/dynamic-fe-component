<template>
  <div class="catalog">
    <v-container class="catalog__frame">
      <p>Our Catalog</p>
      <v-row>
        <v-col cols="3" class="catalog__frame--left">
          <div class="catalog__menu">
            <p class="catalog_noidung--itle">Filling</p>
            <p class="catalog_noidung--detail">
              You can choose one of topping for the cake
            </p>
            <ul>
              <li>Snickers</li>
              <li>Red velvet</li>
              <li>Cream cheese</li>
              <li>Cherry bomb</li>
              <li>Berry</li>
              <li>Bounty</li>
            </ul>
            <a href="#" class="order-button">To Order</a>
          </div>
        </v-col>
        <v-col cols="9" class="catalog__frame--right">
          <v-card>
            <v-tabs
              v-model="tab"
              color="deep-purple-accent-4"
              align-tabs="center"
            >
              <v-tab :value="1">Cakes</v-tab>
              <v-tab :value="2">Cupcakes</v-tab>
              <v-tab :value="3">Cookies</v-tab>
            </v-tabs>
            <v-window v-model="tab">
              <v-window-item v-for="n in 3" :key="n" :value="n">
                <v-container fluid>
                  <v-row>
                    <v-col v-for="i in 6" :key="i" cols="12" md="4">
                      <v-img
                        class="bg-white"
                        width="100̀%"
                        height="auto"
                        :src="`https://picsum.photos/500/300?image=${
                          i * n * 5 + 10
                        }`"
                        :lazy-src="`https://picsum.photos/10/6?image=${
                          i * n * 5 + 10
                        }`"
                        aspect-ratio="1"
                      ></v-img>
                    </v-col>
                  </v-row>
                </v-container>
              </v-window-item>
            </v-window>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    tab: null,
  }),
};
</script>

<style scoped>
.catalog {
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

.catalog__frame--left {
  background-color: #9f0311;
}

.menu {
  background-color: #b71c1c;
  color: white;
  width: 300px;
  padding: 20px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  border-radius: 8px;
  margin: 50px auto;
}

.catalog__menu ul {
  list-style-type: none;
  padding: 0;
}
.catalog__menu li {
  padding: 8px 0;
  border-bottom: 1px solid #f05545;
  text-align: center;
}
.catalog__menu li:last-child {
  border: none;
}
.catalog__img {
  padding: 0;
  margin: 0px;
}

.order-button {
  background-color: #f05545;
  color: white;
  padding: 10px 20px;
  text-align: center;
  display: block;
  margin: 20px auto;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  text-decoration: none;
  font-size: 18px;
}

@media (min-width: 600px) and (max-width: 1024px) {
  .v-col {
    flex-basis: 100%;
    max-width: 100%;
  }
  .catalog__frame--left,
  .special-offer__frame--left {
    order: 2;
  }
  .catalog__frame--right,
  .special-offer__frame--right {
    order: 1;
  }
}

@media (max-width: 599px) {
  .v-col {
    flex-basis: 100%;
    max-width: 100%;
  }
}
.order-button:hover {
  background-color: #e53935;
}
</style>
