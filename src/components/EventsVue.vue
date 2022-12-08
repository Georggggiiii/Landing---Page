<template>
    <div class="wedding-events">
        <h1 class="h1">Wedding Events</h1>
        <div class="img">
            <img src="../assets/section_shape.png" alt="">
        </div>
    </div>
    <div class="center-images">
    <div class="wedding-images" v-for="(image,index) in images" :key="index">
        <img :src="image.url" alt="">
        <span>{{image.date}}</span>
        <h3>{{image.title}}</h3>
        <p>Typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when unknown printer took a galley</p>
        <a href="#">Read More...</a>
    </div>
</div>
</template>

<script>
export default {
data() {
    return {
        images: [
            {
                id:1,
                url:'https://preview.uideck.com/items/wedding-day/assets/images/event-1.jpg',
                title:"Bride Shower",
                date:"02 Feb 2023"

                
            },
            {
                id:2,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/event-2.jpg",
                title:"Bride Shower",
                date:"05 Feb 2023"
            },
            {
                id:3,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/event-3.jpg",
                title:"Bachelor Party",
                date:"07 Feb 2023"
            }
         
        ]
    }
}
}
</script>

<style scoped>
body {
    overflow-x: none;
}
.img {
    text-align: center;
    justify-content: center;
    display: grid;
}
.wedding-events .h1 {
    text-align: center;
    margin-top: 100px;
    color: #D59A57;
    font-family: 'Times New Roman', Times, serif;
}
.center-images {
    justify-content: center;
   display: grid;
   grid-template-columns: auto auto auto;
    margin-top: 50px;
}
.wedding-images {
    width: 372px;
    height: 600px;

}
.wedding-images img {
    border-radius: 10px;
}
.wedding-images span {
    font-size: 16px;
    color: #747E88;
    font-weight: 700;
}
.wedding-images h3 {
    font-size: 30px;
    color: #38424D;

    font-family: 'Times New Roman', Times, serif;
}
.wedding-images p {
    width: 270px;
    line-height: 25px;
    color: #747E88;
    font-weight: 400;
    font-size: 16px;
}
.wedding-images p,h3,span, a {
    padding-left: 20px;
}
.wedding-images a {
    text-decoration: none;
    color: #747E88;
    font-weight: 400;

}
.wedding-images a:hover {
    color: #D59A57;
    transition: 0.3s all;
}
@media only screen and  (max-width:1200px) {
    .wedding-images {
        text-align: center;
        justify-content: center;
        display: grid;
       width: 330px;
    }
    .wedding-images img {
        width: 300px;
    }
    .wedding-images p {
        width: 200px;
        margin-top: -30px;
    }
    .wedding-images h3 {
        transform: translateX(-50px);
        font-size: 25px;
    }
}
@media only screen and (max-width:1000px) {
    .center-images {
        display: grid;
        grid-template-columns: auto;
    }
    .wedding-images img {
        width: 400px;
    }
    .wedding-images p {
      width: 260px;
        margin-left: -10px;
    }
    .wedding-images span {
        transform: translateX(-140px);

    }
    .wedding-images h3 {
        margin-top: -5px;
        margin-left: -120px;
    }
    
    .wedding-images a {
        transform: translate(-145px,-10px);
    }
}
@media only screen and (max-width:767px) {
 .wedding-images {
    justify-content: center;
    display: grid;
 }
    .wedding-images img {
        width: 500px;
        margin-top: 20px;
        padding:0 20px;
        overflow-y: hidden;
    }
    
    .wedding-images p {
      width: 400px;
      margin-top: 5px;
    }
    .wedding-images span {
       line-height: 50px;
       transform: translateX(-190px);
     width: 500px;


    }
    .wedding-images h3 {
        margin-top: -5px;
        margin-left: -220px;
    }
    
    .wedding-images a {
        transform: translate(-180px,10px);

    }
    .wedding-images:nth-child(2) {
        margin-top: 100px;
    }
    .wedding-images:nth-child(3) {
        margin-top: 100px;
    }
}

</style>