<template>
  <div>
    <div
    >
      <v-row style="background: blue" justify="center">
        <v-col style="background: orange" cols="10" lg="10" md="10" sm="10">
          <center>
            <v-card>
              <v-col style="background: pink" cols="6" lg="6" md="6" sm="6">
                <v-text-field
                  label="Outlined"
                  single-line
                  outlined
                ></v-text-field>
              </v-col>
              <v-col style="background: pink" cols="6" lg="6" md="6" sm="6">
                <h3>DIARIO</h3>
              </v-col>
            </v-card>
          </center>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  mounted() {
   alert("cxc");
  },
  data() {
    return {
      apps: [
    
       
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
