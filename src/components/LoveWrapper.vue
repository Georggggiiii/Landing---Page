<template>
<div class="flex">

    <div class="text">
        <h3> We Met For The First Time</h3>
        <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna nose aaliquyam erat, sed diam voluptua. At vero eos et accusam justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea timata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum.</p>
    </div>

        <div class="middle two">
            <p><i class="fa-solid fa-heart"></i>7 May 21</p>
        </div>


        <div class="image">
            <img src="https://preview.uideck.com/items/wedding-day/assets/images/love-1.jpg" alt="">
        </div>

</div>


<div class="flex">
    <div class="text">
    <h3>We AreFirst Dating</h3>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna nose aaliquyam erat, sed diam voluptua. At vero eos et accusam justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea timata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum.</p>
</div>
   

    <div class="middle two">
        <p><i class="fa-solid fa-heart"></i>7 May 21</p>
    </div>

    <div class="image ">
        <img src="https://preview.uideck.com/items/wedding-day/assets/images/love-2.jpg" alt="">
    </div>
 


</div>


<div class="flex">
 
    <div class="text">
    <h3>We Live Together</h3>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna nose aaliquyam erat, sed diam voluptua. At vero eos et accusam justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea timata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum.</p>
</div>


    <div class="middle two">
        <p><i class="fa-solid fa-heart"></i>7 May 21</p>
    </div>



<div class="image">
        <img src="https://preview.uideck.com/items/wedding-day/assets/images/love-3.jpg" alt="">
    </div>

</div>
</template>
<style scoped>

.text h3 {
    color: #D59A57;
    font-family: 'Times New Roman', Times, serif;
    font-size: 30px;
}
.text p {
    width: 400px;
    opacity: 0.7;
    line-height: 20px;
}
.flex {
    margin-top: 50px;
    display: flex;
    justify-content: center;
    position: relative;
    overflow: hidden;
}
.flex .image img {
    border-radius: 13px;
}
.flex::before {
    width: 1px;
    height: 115%;
    position: absolute;
    content: '';
    background-color: #D59A57;
    top: 0;
transform: translateX(-62px);
    justify-content: center;
    text-align: center;
    display: grid;
}
.middle {
    width: 10%;
    text-align: center;
    justify-content: center;
    display: grid;
}
.middle p {
    width: 40px;
    position: relative;
    color: #D59A57;
    border: 1px solid #D59A57;
    border-radius: 50px;
    font-size: 15px;
    padding: 2px;
    line-height: 35px;
    padding-bottom: 32px;
    padding-top: 62px;
    background-color: #fff;
    margin: 0 auto;
    height: 130px;
    justify-content: center;
    text-align: center;
    display: grid;
}
.middle , .text {
    margin-top: 5%;
}
.middle p i {
    width: 43px;
    height: 40px;
    line-height: 38px;
    text-align: center;
    border: 1px solid #D59A57;
    border-radius: 50%;
    color: #D59A57;
    position: absolute;
    top: -1px;
    left: -1px;
}
.fa-solid fa-heart::before {
    content: "\eadf";
}

@media only screen and (max-width:1400px) {

.image img {
    width: 400px;
}
.text p {
    width: 380px;
}
.flex::before {
    transform: translateX(-10px);
}
}
@media only screen and (max-width:930px) {

.image img {
    width: 330px;
}
.text p {
    width: 350px;
}

 }
 .flex {
   justify-content: center;
   text-align: center;
 }

 @media only screen and (max-width:925px) {
    .flex {
        display: grid;
        justify-content: center;
        text-align: center;

    }
    .flex::before {
        display: none;
    }

    .two p {
        width: 400px;
    height: 40px;
    padding-left: 62px;
    padding-right: 30px;
    padding-top: 0;
    padding-bottom: 0;
    transform: translateX(230px);
    }
    .image img {
    width: 500px;
    margin-top: 30px;
   
}
.text p {
    width: 450px;
}
 }
</style>