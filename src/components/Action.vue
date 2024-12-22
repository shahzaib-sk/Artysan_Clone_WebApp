<template>
  <div class="action">
    <div class="action-span">
        <span></span>Available
    </div>
    <div class="action-h2">The time in nigh, Hero</div>
    <div class="action-p">
        A bit dramatic perhaps, but slots are filling fast - don't miss   your chance to join!
    </div>
    <div class="booking-section">
        <div class="button">
            <div class="button-img">
                <img src="../assets/action/call.svg" alt="call">
            </div>
            <div class="button-text">
                <h3>Book a Free intro call <span>→</span></h3>
                <p>Tell us about your projects, and let's find out if Artysan is right for you.</p>
            </div>
        </div>
        <div class="button">
            <div class="button-img">
                <img src="../assets/action/rocket.svg" alt="call">
            </div>
            <div class="button-text">
                <h3>Get Started Today <span>→</span></h3>
                <p>All your design needs streamlined into one monthly membership.</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .action {
        margin-top: 100PX;
    }
    .action-span {
        text-align: center;
    }
    .action-span span {
        height: 8px;
        width: 8px;
        background-color: rgb(65, 189, 65);
        border-radius: 50%;
        display: inline-block;
        margin-right: 12px;
    }
    .action-h2 {
        margin: 18px 0;
        font-size: 56px;
        font-weight: bold;
    }
    .action-p {
        font-size: 16px;
        word-spacing: 1px;
        letter-spacing: 1px;
    }
    .booking-section {
        margin: 60px auto;
        display: flex;
        justify-content: center;
        width: 1200px;
    }
    .button {
        border: 1px solid grey;
        border-radius: 15px;
        display: flex;
        align-items: center;
        margin: 0 12px;
        padding: 8px 18px;
        width: 400px;
        box-shadow: 0 3px 0 0 rgb(218, 218, 218);
        transition: all .3s;
    }
    .button-img {
        margin-right: 22px;
    }
    .button-text {
        text-align: left;
    }
    .button-text span{
        margin-left: 12px;
        font-weight: bold;
        font-size: 22px;
    }
    .button:hover {
        cursor: pointer;
        box-shadow: 1px 3px 1px 2px rgb(94, 93, 93);
    }
</style>