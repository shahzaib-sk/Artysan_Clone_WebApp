<template>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <div class="footer">
    <div class="footer-left">
        <img src="../assets/Header/artysanlogo.svg" alt="">
        <p>© Artysan 2024. All rights reserved</p>
    </div>
    <div class="footer-right">
        <span>
            <i class="fa-brands fa-facebook"></i>
            <i class="fa-regular fa-envelope"></i>
            <i class="fa-brands fa-x-twitter"></i>
            <i class="fa-brands fa-linkedin"></i>
        </span>
        <p>Terms of service Privacy policy</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .footer {
        border-top: 1px solid rgb(223, 220, 220);
        margin-left: 32px;
        margin-right: 32px;
        margin-top: 102px;
        display: flex;
        justify-content: space-between;
    }
    .footer-left {
        text-align: left;
        margin-top: 30px;
    }
    .footer-left img {
        width: 120px;
    }
    .footer-right {
        margin-top: 30px;
    }
    .footer-right span {
        font-size: 20px;
    }
    .footer-right span i {
        padding: 0px 5px;
    }
</style>