<template>
    <div class="grid">
        <div class="main-contact-form">
    <div class="contact-form">
    <h3>You Are Invited!</h3>
    <img src="./section_shape.png" alt="">
    <p>Recently cut out of an illustrated magazine and housed in a nice, gilded frame. It showed a lady fitted out with a fur hat</p>
    </div>
    <div class="inputs">
        <input type="text" placeholder="Name">
        <input type="text" placeholder="Email">     
        <input type="text" class="line" placeholder="Number Of Guest">     
        <input type="text" class="line" placeholder="Attending On">        
    </div>
    <textarea name="massage" class="massage" placeholder="Massage"></textarea>    
    <div class="confirm-btn">
<button class="btn">Confirm Invitation</button>
</div> 
</div>
</div>
</template>

<style scoped>
.grid {
    margin-top: 200px;

    justify-content: center;
    display: grid;

}
.main-contact-form {
    background-color: white;

    justify-content: center;
   text-align: center;
    width: 1000px;
    display: grid;
    height: 100%;
}
.contact-form {
    justify-content: center;
}
.contact-form h3 {
    color: #D59A57;
    font-size: 35px;
    font-family: 'Times New Roman', Times, serif;
}
.contact-form p {
    width: 600px;
    opacity: 0.6;
    line-height: 25px;
}
.inputs {
    display: grid;
    grid-template-columns: auto auto;
    margin-right: -15px;
    margin-left: -15px;
    margin-top: 20px;
}
.inputs input {
    padding: 0 25px;
    border-radius: 5px;
    height: 55px;
    color: #747E88;
    width: 80%;
    border:1px solid rgb(219, 219, 219);
    font-weight: bold;
}
 .massage {
    resize: none;
    height: 185px;
    border-radius: 5px;
    color: #747E88;
    width: 100%;
    border:1px solid rgb(219, 219, 219);
    margin-top: 20px;
    transform: translateX(-13px);
    padding-left: 20px;
}
.inputs .line {
    margin-top: 20px;

}
.btn {
    text-align: center;
    padding: 0 40px;
    background-color: #D59A57;
    color: white;
    line-height: 46px;
    border: none;
    border-radius: 5px;
    font-weight: 500;
    font-size: 16px;
    cursor: pointer;
}
.confirm-btn {
    justify-content: center;
    display: grid;
    margin-top: 30px;
}
.btn:hover {
    background-color: white;
    color: #D59A57;
    border:1px solid #D59A57;
    transition: all 0.4s ease-out 0s;
}

@media only screen and (max-width:1020px) {

    .inputs input {
        width: 200px;
    }
    .main-contact-form {
        width: 700px;
    }
    .massage {
        height: 150px;
    }
    .contact-form p {
    width: 500px;
    opacity: 0.6;
    line-height: 25px;
}
}
@media only screen and (max-width:760px) {
    .inputs {
        display: grid;
        grid-template-columns: auto;
    }
.inputs input {
    width: 73%;
    margin-left: 50px;
    font-size: 17px;
}
.inputs input:nth-child(2) {
    margin-top: 15px;
}
.main-contact-form {
    width: 500px;
}
.massage {
    height: 100px;
    margin-left: 50px;
    width: 83%;
    font-size: 17px;
}
.contact-form p {
width: 500px;
opacity: 0.6;
line-height: 25px;
}
}
@media only screen and (max-width:460px) {
    .inputs input {
    width: 80%;
    margin-left: 30px;
    font-size: 17px;
}
.inputs input:nth-child(2) {
    margin-top: 15px;
}
.main-contact-form {
    width: 500px;
}
.massage {
    height: 100px;
  margin-left: 30px;
    width: 97%;
    font-size: 17px;
}
.contact-form p {
width: 300px;
opacity: 0.6;
line-height: 25px;
}
}
</style>