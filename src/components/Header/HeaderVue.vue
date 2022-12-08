<template>
    <div id="home" class="photo bg_cover">
    <div class="header">
        <img class="header-img" src="./logo-2.png" alt="">
        <a class="non-resp" href="#home">Home</a>
        <a class="non-resp" href="#lovely">Couple</a>
        <a class="non-resp" href="#story">Story</a>
        <a class="non-resp" href="#gallery">Gallery</a>
        <a class="non-resp" href="#events">Event</a>
        <a class="non-resp" href="#rsvp">RSVP</a>
     
            <button @click="open = !open" class="navbar">
                <span class="toggler-icon"></span>
                <span class="toggler-icon"></span>
                <span class="toggler-icon"></span>
            </button>
            <div v-if="open" class="button-links">
                <a href="#home">Home</a>
        <a href="#lovely">Couple</a>
        <a href="#story">Story</a>
        <a href="#gallery">Gallery</a>
        <a href="#events">Event</a>
        <a href="#rsvp">RSVP</a>
            </div>
    </div>
    <div class="middlevue">
    <MiddleVue />
</div>
    </div>
    <div id="lovely">
<LovelyText />
</div>
<TimerVue />
<div id="story">
<LoveText />
</div>
<div class="resp">
<LoveWrapper />
</div>

<div id="gallery">
<GalleryVue />
</div>

<div id="events">
<EventsVue />
</div>
<div id="rsvp">
<ContactForm />
</div>
<FooterComp />
    </template>
    
    <script>
    import MiddleVue from '../MiddleVue.vue';
    import LovelyText from '../LovelyText.vue'
    import TimerVue from '../TimerVue.vue';
    import LoveText from '../LoveText.vue';
    import LoveWrapper from '../LoveWrapper.vue';
    import GalleryVue from '../Gallery/GalleryVue.vue'
    import EventsVue from '../EventsVue.vue';
    import ContactForm from '../ContactForm/ContactForm.vue';
    import FooterComp from '../Footer/FooterComp.vue';
    
    export default {
        data() {
        return {
            open:false,
        }
    },
        components: {
        MiddleVue,
        LovelyText,
        TimerVue,
        LoveText,
        LoveWrapper,
        GalleryVue,
        EventsVue,
        ContactForm,
        FooterComp
  
    }
    }
    </script>
    
    <style scoped>
  .navbar {
    padding: 0.25rem 0.75rem;
    font-size: 1.25rem;
    line-height: 1;
    background-color: transparent;
    border: 1px solid transparent;
    border-radius: 0.25rem;
  }
 .navbar .toggler-icon {
    width: 30px;
    height: 2px;
    background-color: #fff;
    display: block;
    margin: 5px 0;
    position: relative;
    -webkit-transition: all 0.3s ease-out 0s;
    -moz-transition: all 0.3s ease-out 0s;
    -ms-transition: all 0.3s ease-out 0s;
    -o-transition: all 0.3s ease-out 0s;
    transition: all 0.3s ease-out 0s;
 }
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        overflow-x: hidden;
    }
    body {
        scroll-behavior: smooth;
    }
    .header {
        text-align: center;
    }
    .header .header-img {
        margin-top: 5px;
        width: 5%;
        margin-right: 23%;
    }
    .header .non-resp {
        text-decoration: none;
        color: white;
       text-align: center;
       float: center;
       margin: 20px 20px;
       font-size: 17px;
       font-weight: bold;
    }
    .photo {
        background-image: url(./slider-1.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center center;
        height: 900px;
        position: relative;
        left: -8px;
        top: -8px;
        z-index: 999;
        overflow-y: hidden;
    }

    
    @media only screen and (max-width: 1600px) {
        .photo {
            width: 100%;
        }
        img {
            width: 100%;
        }
    }
    
    @media only screen and (max-width: 1000px) {
        .photo {
            width: 105%;
            overflow-x: hidden;
        }
        .header .non-resp {
            display: none;
        }
        .header .header-img {
            transform: translateX(-200px);
            width: 80px;
            margin-top: 20px;
        }
        
        .navbar {
            float: right;
            margin-top: 20px;
            transform: translateX(-60px);
        }
       
    .button-links {
        display: grid;
        float: right;
        margin-top: 50px;
    }
    .button-links a {
        text-decoration: none;
        color: white;
        padding-bottom: 10px;
        margin-top: 10px;
    }
    }
    .middlevue {
        margin-top: -50px;
    }

    @media only screen and (min-width: 1000px) {
        button {
            display: none;
        }
        .button-links {
            display: none;
        }
    }
@media only screen and (max-width:720px) {
    .photo {
            width: 110%;
            overflow-x: hidden;
        }

        .header .header-img {
            transform: translateX(-100px);
            width: 80px;
            margin-top: 20px;
        }
     
}
</style>
