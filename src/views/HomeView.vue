<template>
  <v-app
    id="inspire"
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
    <SideBar />
    <v-container>
      <NavBar />
      <v-row>
        <v-col cols="12" sm="8">
          <v-row>
            <v-col cols="12" sm="12">
              <OverView />
            </v-col>
            <v-col cols="12" sm="12">
              <MoneyPart />
            </v-col>
            <v-col cols="12" sm="12">
              <PaymentPart />
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" sm="4">
          <CardPart />
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
import SideBar from "@/components/SideBar.vue";
import NavBar from "@/components/NavBar.vue";
import OverView from "@/components/OverView.vue";
import MoneyPart from "@/components/MoneyPart.vue";
import PaymentPart from "@/components/PaymentPart.vue";
import CardPart from "@/components/CardPart.vue";

export default {
  name: "HomePage",

  components: {
    SideBar,
    NavBar,
    OverView,
    MoneyPart,
    PaymentPart,
    CardPart,
  },
};
</script>

<style>
.v-btn.withoutupercase {
  text-transform: none !important;
}
.v-btn:not(.v-btn--round).v-size--small {
  min-width: 30px !important;
  padding: 0 5px !important;
}
</style>
