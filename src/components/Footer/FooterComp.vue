<template>
    <div class="container">
        <div class="wedding-day-picture">
<img src="./logo-2.png" alt="">
<h3 class="title">Michael <span>&</span> Jessica</h3>
<div class="link-tags">
<a href="#">Home</a>
    <a href="#">Couple</a>
    <a href="#">Story</a>
    <a href="#">Gallery</a>
    <a href="#">Event</a>
    <a href="#">RSVP</a>
</div>
<div class="orange-line">
    
</div>
<div class="designed">
<p>Designed And Developed by <a class="uideck" href="#">Uideck</a></p>
</div>
</div>

<div class="footer">
    <img class="footer-img" src="./shape-1.png" alt="">
</div>

    </div>
</template>

<style scoped>
.container {
    background-color: #FCF4EC;
    position: relative;
    z-index: 9;
    overflow: hidden;
    margin-top: 200px;
}
.footer .footer-img {
    width: 130px;
    opacity: 0.31;
    margin-top: -200px;
}
.wedding-day-picture{
    margin-top: 10%;
    text-align: center;
    justify-content: center;
    display: grid;

}
.wedding-day-picture img {
    transform: translateX(60%);
}

.wedding-day-picture .title{
    font-family: 'Times New Roman', Times, serif;
    font-size: 52px;
    color: #38424D;
}
.wedding-day-picture span {
    color: #D59A57;
    font-family: 'Times New Roman', Times, serif;
}
a {
    text-decoration: none;
}
.link-tags {
   display: grid;
   grid-template-columns: auto auto auto auto auto auto;
   justify-content: center;

}
.link-tags a {
    color: #38424D;
    padding-right: 50px;
}
.orange-line {
    width: 200%;
    height: 2px;
    background-color: #D59A57;
    margin-top: 15%;
    justify-content: center;
    text-align: center;
    margin-left: -260px;
}
.designed {
    margin-top: 10%;
    font-weight: bold;
    opacity: 0.5;
}
.designed a {
    color: #D59A57;
}
@media only screen and (max-width:1275px) {
    .orange-line {
        width: 150%;
        transform: translateX(140px);
    }
}
@media only screen and (max-width:1000px) {
    .orange-line {
        width: 110%;
        transform: translate(250px,30px);
    }
}
@media only screen and (max-width:770px) {
    .orange-line {
        width: 100%;
        transform: translate(60%,30px);
    }
    .link-tags {
   display: grid;
   grid-template-columns: auto auto auto auto auto;
   justify-content: center;

}
.wedding-day-picture img {
    width: 150px;
transform: translateX(165px);
}
.wedding-day-picture .title{
    font-family: 'Times New Roman', Times, serif;
    font-size: 35px;
    color: #38424D;
}
.link-tags a:nth-child(6) {
transform: translate(208%,5px);
}
}
@media only screen and (max-width:570px) {
    .orange-line {
        width: 100%;
        transform: translate(60%,30px);
    }
    .link-tags {
   display: grid;
   grid-template-columns: auto auto auto auto;
   justify-content: center;

}
.link-tags a:nth-child(6) {
transform: translate(98%,5px);
}
.link-tags a:nth-child(5) {
transform: translate(105%,5px);
}
}

</style>