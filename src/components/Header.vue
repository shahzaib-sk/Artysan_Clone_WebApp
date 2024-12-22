<template>
  <div class="header-container">
    <!-- NAV BAR -->
    <div class="nav-bar"
        :class="{ sticky: isSticky }"
        ref="navbar">
        <div class="nav-logo">
            <img src="../assets/Header/artysanlogo.svg" alt="Artysan Logo">
        </div>
        <div class="nav-instr">
            <a href="#" class="links">Benefits</a>
            <a href="#" class="links">How it works</a>
            <a href="#" class="links">Services</a>
            <a href="#" class="links">Pricing</a>
            <a href="#" class="links">FAQs</a>
        </div>
        <div class="nav-btn">
            <button>Login</button>
        </div>
    </div>

    <!-- HEADER -->
    <div class="header">
        <div class="header-h1">
            Award-winnig design partner for <br>
            your business, on demand
        </div>
        <div class="header-p">
            All your design needs streamlined into one single flat monthly membership: <br>
            Brand, Website, Products and everything in between - it's kinda magic.
        </div>
        <div class="header-btn">
            <button>See plans</button>
        </div>
        <div class="header-span">
            <span class="span-dot"></span>Available
        </div>
        <div class="header-img">
            <img src="../assets/Header/header1.avif">
            <img src="../assets/Header/header3.avif">
            <img src="../assets/Header/header2.avif">
            <img src="../assets/Header/header1.avif">
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            isSticky: false,
        };
    },
    methods: {
        handleScroll() {
        this.isSticky = window.scrollY > 0; 
        }
    },
    mounted() {
        window.addEventListener('scroll', this.handleScroll);
    },
    beforeDestroy() {
        window.removeEventListener('scroll', this.handleScroll);
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&display=swap');

    /* .header-container {
        height: 100vh;
    } */
/* NAV BAR STYLING */
    .nav-bar {
        display: flex;
        justify-content: space-around;
        align-items: center;
        /* background-color: crimson; */
        padding: 16px;
    }
    .nav-bar.sticky {
        display: flex;
        align-items: center;
        position: fixed;
        top: 0;
        /* width: 100%; */
        z-index: 1000;
        background-color: white;
        max-width: 800px;
        border-radius: 45px;
        margin: 12px auto;
        left: 0;
        right: 0;
        /* padding: 10px; */
        box-shadow: 0px 2px 0px 3px black;
        transform: translateY(5%);
        transition: 0.3s ease-in-out;

    }
    .nav-logo {
        height: 35px;
        width: 150px;
        cursor: pointer;
    }
    .nav-instr a {
        text-decoration: none;
        color: #111826;
        font-size: 16px;
        padding: 12px;
    }
    .nav-instr a:hover {
        color: #15A0F5;
        transition: all .2s;
    }
    .nav-btn button{
        font-size: 16px;
        padding: 10px 26px;
        border-radius: 22px;
        color: white;
        background: #111826;
    }
    .nav-btn button:hover {
        background: #364151;
        cursor: pointer;
        transition: all .2s;
    }

/* HEADER STYLING */
    .header {
        display: flex;
        flex-direction: column;
        /* background-color: red; */
        text-align: center;
    }
    .header-h1 {
        font-size: 54px;
        font-weight: bold;
        margin-top: 130px;
    }
    .header-p {
        font-size: 22px;
        color: #364157;
        margin: 22px 0;
        line-height: 32px;
    }
    .header-btn button {
        font-size: 18px;
        padding: 16px 26px;
        border-radius: 12px;
        color: white;
        font-weight: bold;
        background: #364151;
        box-shadow: #364151;
        margin: 26px 0;
    }
    .header-btn button:hover {
        background: #394352;
        transition: all .3s;
        cursor: pointer;
    }
    .header-span {
        text-align: center;
    }
    .span-dot {
        height: 8px;
        width: 8px;
        background-color: rgb(65, 189, 65);
        border-radius: 50%;
        display: inline-block;
        margin-right: 12px;
    }
    .header-img {
        margin-top: 100px;
        display: flex;
        width: 100%;
        height: 600px;
        background-color: #EEF2F6;
        overflow: hidden;
    }
    .header-img img {
        width: 200px; 
        height: 100%; 
        object-fit: cover; 
        margin: 0 auto; 
        transform: rotate(35deg) scale(2.5);
        padding: 18px;
        background-color: #EEF2F6;
    }
</style>