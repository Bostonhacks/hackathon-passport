<template>
  <div class="check-in-page">
    <food class="food-icon" />
    <h1 class="h1">Check-in</h1>
    <h2 class="h2">Click one of the buttons below to check-in!</h2>
    <a v-on:click="food" class="text button orange" href="#">FOOD CHECK-IN</a>
    <a v-on:click="event" class="text button orange" href="#">
      EVENT CHECK-IN
    </a>
    <a v-on:click="workshop" class="text button orange" href="#">
      WORKSHOP CHECK-IN
    </a>
  </div>
</template>
<script>
import food from '@/SVG/food.vue';
export default {
  components: {
    food,
  },
  methods: {
    food: () => {
      alert('food');
    },
    event: () => {
      alert('event');
    },
    workshop: () => {
      alert('workshop');
    },
  },
};
</script>

<style>
.text {
  font-family: 'Roboto', sans-serif;
}
.h1 {
  font-family: 'Roboto', sans-serif;
  font-style: normal;
  font-weight: bold;
  font-size: 64px;
  line-height: 75px;
  color: #ec602d;
  text-shadow: -1px 0 black, 0 1px black, 1px 0 black, 0 -1px black;
}
.h2 {
  font-family: Ubuntu, 'times new roman', times, roman, serif;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 23px;
}
.check-in-page {
  align-content: center;
  text-align: center;
  background-color: #fec736;
  display: block;
  flex-direction: column;
}

.button {
  display: block;
  width: 516px;
  height: 130px;
  line-height: 50px;
  padding-right: 30px;
  padding-left: 70px;
  position: relative;
  background-color: rgb(41, 127, 184);
  color: black;
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 15px;
  border-radius: 30px;
  -moz-border-radius: 30px;
  -webkit-border-radius: 30px;
  text-shadow: 0px 1px 0px rgba(0, 0, 0, 0.5);
  -ms-filter: 'progid:DXImageTransform.Microsoft.dropshadow(OffX=0,OffY=1,Color=#ff123852,Positive=true)';
  zoom: 1;
  filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=0,OffY=1,Color=#ff123852,Positive=true);
  -moz-box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.2);
  -webkit-box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.2);
  box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.2);
  -ms-filter: 'progid:DXImageTransform.Microsoft.dropshadow(OffX=0,OffY=2,Color=#33000000,Positive=true)';
  filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=0,OffY=2,Color=#33000000,Positive=true);
  font-size: 30px;
  height: 130px;
  line-height: 130px;
  text-align: center;
}

.button span {
  position: absolute;
  left: 0;
  width: 50px;
  background-color: rgba(0, 0, 0, 0.5);

  -webkit-border-top-left-radius: 5px;
  -webkit-border-bottom-left-radius: 5px;
  -moz-border-radius-topleft: 5px;
  -moz-border-radius-bottomleft: 5px;
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;
  border-right: 1px solid rgba(0, 0, 0, 0.15);
}

.button:hover span,
.button.active span {
  background-color: rgb(0, 102, 26);
  border-right: 1px solid rgba(0, 0, 0, 0.3);
}

.button:active {
  margin-top: 2px;
  margin-bottom: 13px;
  -moz-box-shadow: 0px 1px 0px rgba(255, 255, 255, 0.5);
  -webkit-box-shadow: 0px 1px 0px rgba(255, 255, 255, 0.5);
  box-shadow: 0px 1px 0px rgba(255, 255, 255, 0.5);
  -ms-filter: 'progid:DXImageTransform.Microsoft.dropshadow(OffX=0,OffY=1,Color=#ccffffff,Positive=true)';
  filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=0,OffY=1,Color=#ccffffff,Positive=true);
}

.button.orange {
  background: #ffffff;
}

.btn-active {
  background: #ffffff;
}

.food-icon {
  position: absolute;
  z-index: 1;
}
</style>
