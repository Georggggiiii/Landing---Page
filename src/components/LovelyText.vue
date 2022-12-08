<template>
    <div id="couple" class="text">
        <h1>Lovely Couple</h1>
        <img  class="section-image" src="../assets/section_shape.png" alt="fff">
    </div>
   <div class="flex">
    <div class="single-image-michael">
        <img src="https://preview.uideck.com/items/wedding-day/assets/images/couple-1.jpg" alt="">
        <div class="image-text">
            <h4>Michael Smith</h4>
            <p>Hi I am Michael Smith, dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries.</p>
            <div class="social-logos">
                <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
            </div>
        </div>
    </div>
    <div class="single-image-michael">
        <img src="https://preview.uideck.com/items/wedding-day/assets/images/couple-2.jpg" alt="">
        <div class="image-text">
            <h4>Jessica Jones</h4>
            <p>Hi I am Jessica Jones, dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries.</p>
            <div class="social-logos">
                <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
            </div>
        </div>
    </div>
   </div>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
.text h1 {
    font-family: 'Lobster', cursive;
    text-align: center;
    color: #D59A57;
    font-size: 40px;
    margin-top: 100px;
}
.text {
    justify-content: center;
    display: grid;
}
.flex {
    display: flex;
    justify-content: center;
    margin-top: 50px;
}
.single-image-michael {
  margin-right: 30px;
}
.single-image-michael img{
border-radius: 12px;
}
.image-text {
background-color: white;
border-radius: 10px;
text-align: center;
transform: translateY(-130px);
width: 90%;
    margin: 0 auto;
    z-index: 5;
}
.image-text h4 {
    font-family: 'Lobster', cursive;
    color: #D59A57;
    font-size: 40px;
    margin-bottom: 30px;
    padding-top: 40px;
}
.image-text p {
    width: 400px;
color: darkgrey;
line-height: 25px;
margin-left: 40px;
}
.social-logos i{
    width: 35px;
    height: 35px;
    line-height: 33px;
    text-align: center;
    border: 1px solid #747E88;
    color: #747E88;
    font-size: 16px;
    border-radius: 50%;
    -webkit-transition: all 0.3s ease-out 0s;
    -moz-transition: all 0.3s ease-out 0s;
    -ms-transition: all 0.3s ease-out 0s;
    -o-transition: all 0.3s ease-out 0s;
    transition: all 0.3s ease-out 0s;
    margin-right: 10px;
}
@media only screen and (max-width:1200px){
    .flex {
        text-align: center;
        justify-content: center;
    }
    .single-image-michael{
background-color: white;
border-radius: 10px;
text-align: center;
width: 40%;
    z-index: 5;
    justify-content: center;
}
.image-text {
    width: 85%;
}
.single-image-michael img {
    width: 450px;
}
.image-text p {
    width: 300px;
    transform: translateX(50px
    );
}
}
@media only screen and (max-width:1000px) {
    .flex {
        text-align: center;
        justify-content: center;
    }
    .single-image-michael{
background-color: white;
border-radius: 10px;
text-align: center;
width: 40%;
    z-index: 5;
    justify-content: center;
}
.single-image-michael img {
    width: 350px;
}
.image-text p {
    width: 230px;

}
}
@media only screen and (max-width:770px) {
    .flex {
        display: grid;
    }
    .flex {
        text-align: center;
        justify-content: center;
    }
    .single-image-michael{
background-color: white;
border-radius: 10px;
text-align: center;
width: 100%;
    z-index: 5;
    justify-content: center;
}
.single-image-michael img {
    width: 500px;
}
.image-text p {
    width: 400px;

}
}
</style>