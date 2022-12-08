<template>
    <div class="gallery-text">
        <h1 class="h1-text" >Our Love Gallery</h1>
        <div class="img">
            <img src="./section_shape.png" alt="">
    </div>
    </div>
<div class="images-grid">
<div class="images" v-for="(image,index) in images" :key="index">
   <img class="image-grid" :src="image.url" alt="">
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
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-1.jpg"
            },
            {
                id:2,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-2.jpg"
            },
            {
                id:3,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-3.jpg"
            },
            {
                id:4,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-4.jpg"
            },
            {
                id:5,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-5.jpg"
            },
            {
                id:6,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-6.jpg"
            },
            {
                id:7,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-7.jpg"
            },
            {
                id:8,
                url:"https://preview.uideck.com/items/wedding-day/assets/images/gallery-8.jpg"
            }
        ]
    }
}
}
</script>

<style scoped>
* {
    overflow-x: none;
}
h1 {
    text-align: center;
    margin-top: 100px;
    color: #D59A57;
    font-family: 'Times New Roman', Times, serif;
}

.img {
    text-align: center;
    justify-content: center;
    display: grid;
}
.images-grid {
    text-align: center;
    display: grid;
    grid-template-columns: auto auto auto auto;
    margin-top: 50px;
}
.images {
    overflow-x: hidden;
}
@media only screen and (max-width:1920px) {
.images-grid img {
    width: 100%;
}
}
@media only screen and (max-width:1500px) {
.images-grid img {
    width: 100%;
}
}
@media only screen and (max-width:1000px) {
.images-grid {
    display: grid;
    grid-template-columns: auto auto;
}
.images img {
    width: 100%;
}
}
@media only screen and (max-width:930px) {
    .images-grid img {
   width: 100%;
}
}
@media only screen and (max-width:580px) {
    .images-grid img {
    width: 100%;
}
.images-grid {
    display: grid;
    grid-template-columns: auto;
}
}
</style>