<template>
  <div class="services">
    <div class="service-span">Services</div>
    <div class="service-h2">If you can dream it, we can desgin it</div>
    <div class="service-p">Logos, websites, interfaces and everything you need. We've got your back.</div>
    <div class="services-images">
        <div class="img">
            <img src="../assets/Services/logoss.svg" alt="logo">
            <p>Logos</p>
        </div>
        <div class="img">
            <img src="../assets/Services/brand.svg" alt="logo">
            <p>Brand guides</p>
        </div>
        <div class="img">
            <img src="../assets/Services/graphic.svg" alt="logo">
            <p>Graphic assets</p>
        </div>
        <div class="img">
            <img src="../assets/Services/decks.svg" alt="logo">
            <p>Pitch decks</p>
        </div>
        <div class="img">
            <img src="../assets/Services/Landing.svg" alt="logo">
            <p>Landing pages</p>
        </div>
        <div class="img">
            <img src="../assets/Services/Websites.svg" alt="logo">
            <p>Websites</p>
        </div>
        <div class="img">
            <img src="../assets/Services/webflow.svg" alt="logo">
            <p>Webflow</p>
        </div>
        <div class="img">
            <img src="../assets/Services/copywrite.svg" alt="logo">
            <p>Copywriting</p>
        </div>
        <div class="img">
            <img src="../assets/Services/design.svg" alt="logo">
            <p>Design systems</p>
        </div>
        <div class="img">
            <img src="../assets/Services/mobile.svg" alt="logo">
            <p>Mobile apps</p>
        </div>
        <div class="img">
            <img src="../assets/Services/product.svg" alt="logo">
            <p>Product UI/UX</p>
        </div>
        <div class="img">
            <img src="../assets/Services/logoss.svg" alt="logo">
            <p>Prototypes</p>
        </div>
    </div>
    <div class="services-pictures">
        <img src="../assets/service pictures/data-ethics.png" >
        <img src="../assets/service pictures/worketc.png" >
        <img src="../assets/service pictures/sage-learning.png" >
        <img src="../assets/service pictures/work-folder.png" >
        <img src="../assets/service pictures/opus.png" >
        <img src="../assets/service pictures/alba.png" >
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .service-span {
        color: #175CD3;
        font-weight: bolder;
        font-size: 18px;
        margin-top: 72px;
        margin-bottom: 18px;
    }
    .service-h2 {
        font-size: 48px;
        font-weight: bolder;
        margin-bottom: 18px;
    }
    .service-p {
        font-size: 19px;
        word-spacing: 1px;
        letter-spacing: 1px;
        color: #364A62;
        margin-bottom: 86px;
    }
    /* .services-images {
        display: flex;
        flex-wrap: wrap;
        padding: 0 180px;
        width: 1000px;
        margin: 0 auto;
        
    }
    .img {
        flex: 1 0 30%;
        padding: 26px 0;
        border: 4px solid #EEF2F6;
        border-radius: 12px;   
    }
    .img img{
        width: 60px;
    }  */

.services-images {
    display: flex;
    flex-wrap: wrap;
    padding: 0 180px;
    width: 1000px;
    margin: 0 auto;
    margin-bottom: 95px;
}

.img {
    flex: 1 0 30%;
    padding: 26px 0;
    border: 4px solid #EEF2F6; 
    border-radius: 12px;   
    box-sizing: border-box; 
    transition: all .3s;
}
.img:hover {
    box-shadow: 0px 5px 5px lightgrey;
}

.img:first-child {
    border-left: none; 
}

.img:last-child {
    border-right: none; 
}


.services-images > .img:nth-child(-n+3) {
    border-top: none; 
}

.services-images > .img:nth-last-child(-n+3) {
    border-bottom: none; 
}

.services-images > .img:nth-child(3n + 1) {
    border-left: none; 
}

.services-images > .img:nth-child(3n) {
    border-right: none; 
}

.img {
    margin: 0 -2px; 
}

.img img {
    width: 60px;
}

    .services-pictures {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        width: 1100px;
        margin: 0 auto;
    }
    .services-pictures img {
        width: 100px;
        margin: 12px;
        flex: 0 0 30%;
        border-radius: 18px;
    }
</style>