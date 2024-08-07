<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-grey">Hello,</h1>
              <h1 class="text-white">I'm Fabian Paez</h1>
              <span class="text-grey">Web Developer</span> <br />
              <v-btn tile dark class="text-yellow mt-8" variant="outlined"
                >Contact me</v-btn
              >
            </div>
          </v-col>
          <v-col cols="2">
            <div
              style="
                position: absolute;
                z-index: 9999;
                bottom: 0;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
            >
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="5">
            <div style="position: relative; z-index: 9999" class="mt-16">
              <v-img src="i1.png" contain max-height="300"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" class="mt-16" id="about">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="i3.jpeg" max-height="290"></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
              <h5 class="mt-16">About Me</h5>
              <br/>
              <div style="width: 120px">
                <!-- <v-slider v-model="slider2" color="yellow" label="track-color"></v-slider> -->
              </div>
              <h4 class="mt-n4">
                I'm an enthusiastic student of Web Development
              </h4>
              <p class="text-grey">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Culpa
                reprehenderit soluta, saepe voluptates esse expedita inventore?
                Amet, autem quam id numquam voluptatum distinctio nulla
                similique debitis quae, pariatur fugit? Voluptate?
              </p>
              <br />
              <p class="text-grey">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Culpa
                reprehenderit soluta, saepe voluptates esse expedita inventore?
                Amet, autem quam id numquam voluptatum distinctio nulla
                similique debitis quae, pariatur fugit? Voluptate?
              </p>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <div class="text-center mt-4">
        <div style="width: 120px; margin: 0 auto">
          <!-- <v-slider v-model="slider2" color="yellow" label="track-color"></v-slider> -->          
        </div>
      </div>
      <v-col cols="12" class="padd" id="portfolio">
        <div class="first" id="project">
          <v-row>
            <v-col cols="12">
              <div class="child">
                <v-btn icon="fas fa-laptop" color="#F8DF7E" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Web Development</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet <br /> consectetur adipisicing
                  <br /> elit. Sit, obcaecati.
                </p>
            </div>
            <div class="child">
                <v-btn icon="fas fa-code" color="#F8DF7E" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">App Development</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet <br /> consectetur adipisicing
                  <br /> elit. Sit, obcaecati.
                </p>
            </div>
            <div class="child">
                <v-btn icon="fas fa-wine-glass" color="#F8DF7E" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Drinking Tetrabrik Wine</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet <br /> consectetur adipisicing
                  <br /> elit. Sit, obcaecati.
                </p>
            </div>
            </v-col>            
          </v-row>
          <v-divider></v-divider>
        </div>
      </v-col>
      <v-col cols="12" sm="12" id="services">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#F8DF7E" class="mr-2">All</v-btn>
          <v-btn class="mr-2" variant="tonal">Backend Projects</v-btn>
          <v-btn class="mr-2" variant="tonal">Frontend Projects</v-btn>
        </div>
      </v-col>
      <v-col cols="12" class="imgHover">
        <v-row class="fill-height" align="center" justify="center">
          <template v-for="(item, i) in items" :key="i">
            <v-col cols="12" md="4">
              <v-hover v-slot="{isHovering, props}">
                <v-card :elevation="isHovering ? 12 : 2" :class="{'on-hover' : isHovering}" v-bind="props">
                  <v-img :src="item.img" height="225px" cover></v-img>
                </v-card>
              </v-hover>
            </v-col>
          </template>          
        </v-row>
      </v-col> <br />
      <v-divider></v-divider>
      <v-col cols="12" sm="12" class="px-16" id="contact">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="child">
              <h1>Contact info</h1>
              <v-btn icon="fas fa-map-marker-alt" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">Calle Siempre Viva 123</span><br />
              <v-btn icon="fas fa-phone-alt" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">0800-474-8074</span><br />
              <v-btn icon="fas fa-envelope" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">mandale-mecha@gmail.com</span><br />
            </div>
          </v-col>
          <v-col cols="12" sm="8">
            <h1 class="mt-8">Send you message</h1>
            <v-divider></v-divider>
            <span class="text-caption">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Id eveniet dignissimos soluta atque ex eaque corporis, eligendi nostrum vero minus saepe aliquid, magnam voluptas! Voluptates similique necessitatibus recusandae consequuntur impedit soluta sequi? 
            </span>
            <v-row class="mt-10">
              <v-col cols="12" sm="6">
                <v-text-field label="Name" persistent-hint variant="outlined"></v-text-field>
              </v-col>
              <v-col cols="12" sm="6">
                <v-text-field label="Phone Number" persistent-hint variant="outlined"></v-text-field>
              </v-col>
            </v-row>
            <v-textarea label="Message" persistent-hint variant="outlined"></v-textarea>
            <v-btn color="#F8DF7E" class="mt-2">Submit Now</v-btn>
          </v-col>
        </v-row>
      </v-col>
    </v-container>
    <FooterView />
  </v-app>
</template>

<script>
import { defineComponent } from "vue";

// Components
import FooterView from "@/components/FooterView.vue";
import NavBar from "@/components/NavBar.vue";

export default defineComponent({
  name: "HomeView",

  setup() {
    return {
      slider2: 50,

      items: [
        {
          img: "i4.jpg",
        },
        {
          img: "i5.jpg",
        },
        {
          img: "i6.jpg",
        },
        {
          img: "i7.jpg",
        },
        {
          img: "i8.jpg",
        },
      ],
    };
  },

  components: {
    NavBar,
    FooterView,
  },
});
</script>

<style scoped>
.v-container {
  padding: 16px 0;
}

.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width: 100%;
  color: white;
}

.head:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}

.head:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}

.egg {
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 356px;
  height: 300px;
  background-color: #fbdf7e;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 0%;
}

.first {
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 2rem 2rem;
}

.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}

.imgHover {
  padding: 0 200px;
}

.pre {
  width: 100%;
  height: 380px;
  text-align: center;
  padding: 0 200px;
  background-color: #f5f5f5;
}

.hire {
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #e9e9e9;
  margin-top: -24px;
}

</style>
