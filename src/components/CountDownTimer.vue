<template>
    <p id="demo" class="flex p"></p>
    <div class="counttimer-background">
    <img class="image" src="https://preview.uideck.com/items/wedding-day/assets/images/shape-2.png" alt="">
    </div>
</template>

<script>

// Set the date we're counting down to
var countDownDate = new Date("Feb 7, 2023 15:59:25").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();

  // Find the distance between now and the count down date
  var distance = countDownDate - now;

  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  // Display the result in the element with id="demo"
  document.getElementById("demo").innerHTML = days +  "days " + hours + "hours "
  + minutes + "minutes " + seconds + "seconds ";

  // If the count down is finished, write some text
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "EXPIRED";
  }
}, 1000);

</script>


<style scoped>
#demo {
    width: 800px;
}
.flex {
    width: 50%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-around;
    margin-top: -150px;
    transform: translateX(80px);
    height: 50%;
    color: white;
}
.p {
    width: 100px;
    height: 100px;
    background-color: #D59A57;
    border-radius: 10px;
    font-size: 1.5rem;
    color: white;
    text-align: center;
} 
.flex .spans {
    color: #D59A57;
    font-size: 30px;

}
.counttimer-background .image{
  width: 130px;
  opacity: 0.31;
  position: absolute;
  left:90%;
  margin-top: -10%;
}
@media only screen and (max-width: 1500px) {
      
        #demo {
          width: 600px;
        }
    }
    
    @media only screen and (max-width: 1061px) {
      
      #demo {
        width: 500px;
      }
  }
  @media only screen and (max-width:927px ) {
   .flex {
    transform: translate(-150px,150px);
   }
  }
  @media only screen and (max-width:570px ) {
  #demo {
    width: 300px;
  }
  }
  
</style>