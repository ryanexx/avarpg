<template>
  <div>
    <div class="versoView"
        id="myScroll"
        :style="{
          height: $porcent(this.$screen.h, 65) + 'px',
        }"
      >
      
<v-row style="background: blue;" justify="center">
      <v-col style="background: orange;" cols="10" lg="10" md="10" sm="10">
    <center>
        <v-card>
      <v-col style="background: pink;" cols="6" lg="6" md="6" sm="6">
     <v-text-field
            label="Outlined"
            single-line
            outlined
          ></v-text-field>

  </v-col>
        <v-col style="background: pink;" cols="6" lg="6" md="6" sm="6">
          <h3>DIARIO</h3>

  </v-col>
      </v-card>
    </center>
  </v-col>

</v-row>
       
      
      </div>
    <v-card class="appStyle" style="float: right; background: yellow">
      <h6 class="textAjust">TOOLS</h6>

      <v-card
        class="divApp"
        id="myScroll"
        :style="{
          height: $porcent(this.$screen.h, 62) + 'px',
        }"
      >
        <v-img
          v-for="(app, n) in apps"
          :key="n"
          @click="(active = n), (titleApp = app.name)"
          class="appItemStyle"
          alt="Vuetify Logo"
          contain
          :src="app.icon"
          transition="scale-transition"
        />
      </v-card>
    </v-card>
  </div>
</template>
<script>
export default {
  components: {},
  props: ["sw", "sh"],
  mounted() {},
  data() {
    return {
      apps: [
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0001",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0002",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0013",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0011",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0012",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0023",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0021",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0022",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0043",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0041",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0042",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0063",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0061",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0062",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0073",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0071",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0072",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0083",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0081",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0082",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0093",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0091",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0112",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0113",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
        {
          name: "Welcome",
          icon: require("@/apps/welcome/icon.svg"),
          id: "0111",
          description: "Organizador academico",
          verso: () => import("@/apps/welcome/verso"),
          priority: 0,
        },
        {
          name: "Linkedu",
          icon: require("@/apps/linkedu/icon.svg"),
          id: "0122",
          description: "Organizador academico",
          verso: () => import("@/apps/linkedu/verso"),
          priority: 0,
        },
        {
          name: "Diariomaker",
          icon: require("@/apps/diariomaker/icon.svg"),
          id: "0123",
          description: "Organizador de diarios",
          verso: () => import("@/apps/diariomaker/verso"),
          priority: 0,
        },
      ],
      active: 0,
      dialog: false,
      icons: ["mdi-rewind", "mdi-play", "mdi-fast-forward"],
      transparent: "rgba(255, 255, 255, 0)",
    };
  },
  methods: {
    datachange() {
      alert("cxc");
    },
  },
};
</script>
<style scoped>
.divFree {
  position: absolute;
  margin-bottom: 1rem;
}

.divScreen {
  height: 100%;
  background: rgb(91, 214, 43);
  position: absolute;
}

div.scroll {
  background-color: #fed9ff;
  width: 100%;
  height: 500px;
  overflow: auto;
  text-align: justify;
}

#scrollTools::-webkit-scrollbar {
  width: 5px;
  background-color: #cccccc;
}
#scrollTools::-webkit-scrollbar-thumb {
  background-color: #b03c3f;
  border-radius: 10px;
}
#scrollTools::-webkit-scrollbar-thumb:hover {
  background-color: #bf4649;
  border: 1px solid #333333;
}
#scrollTools::-webkit-scrollbar-thumb:active {
  background-color: #c2f50a;
  border: 1px solid #333333;
}
</style>
