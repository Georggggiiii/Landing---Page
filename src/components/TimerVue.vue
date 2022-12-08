<template>
  <div class="counttimer-background">
    <img class="image" src="https://preview.uideck.com/items/wedding-day/assets/images/shape-1.png" alt="">
  </div>
  <div class="event-date">
    <h3>Event Date</h3>
    <p>20 December 2023</p>
    <img src="../assets/section_shape.png" alt="">
    <div class="flex">
    <CountDownTimer />


  </div>
  </div>
</template>

<script>
import CountDownTimer from './CountDownTimer.vue';
export default {
  components: {
  CountDownTimer
},

}
</script>


<style scoped>
.counttimer-background {
  background-color: #FCF4EC;
  margin-top: 100px;
}
.counttimer-background .image{
  width: 130px;
  opacity: 0.31;
}
.event-date h3 {
  font-family: 'Lobster', cursive;
  font-size: 45px;
    color: #D59A57;
    line-height: 20px;
  
}
.event-date p {
  font-size: 30px;
    line-height: 20px;
    color: #38424D;
}
.event-date {
  margin-top: -230px;
  margin-left: 300px;
}
@media only screen and (max-width: 1500px) {
        .event-date , p , h3 {
          transform: translateX(-80px);
        }
        #demo {
          width: 500px;
        }
      
    }
         
  @media only screen and (max-width: 1002px) {
      
    .event-date h3 {
      font-size: 35px;
    }
    .event-date p {
      font-size: 25px;
    }
    .event-date img {
      transform: translateX(-70px);
    }
    .flex {
      margin-top: 30px;
    }
  }

</style>