<template>
  <div class="review-section">
    <div class="review-h2">You'll be in good company</div>
    <div class="review-p">Hear it from those know best.</div>
    <div class="customer-review">
        <div class="review">
            <div class="review-intro">
                <div class="customer-img">
                    <img src="../assets/customers/ben.jpeg" alt="Customer">
                </div>
                <div class="customer-text">
                    <h4>Beng Aung</h4>
                    <p>Cheif Risk Officer, Sage</p>
                </div>
            </div>
            <div class="review-rating">
                ★★★★★ 
            </div>
            <div class="review-comment">
                It's been pleasure working with you <span>@Mass</span>, especially how you have turned our usually unstructured ideas into something so unique and engaging for our customers
            </div>
            
        </div>
        <div class="review">
            <div class="review-intro">
                <div class="customer-img">
                    <img src="../assets/customers/gustavo.jpeg" alt="Customer">
                </div>
                <div class="customer-text">
                    <h4>Gustavo Zeidan</h4>
                    <p>CISCO, Sage</p>
                </div>
            </div>
            <div class="review-rating">
                ★★★★★
            </div>
            <div class="review-comment">
                It has been an absolute deslight towork with you <span>@Mass.</span> I cannot wait to see what you can do next as we evolve our mission to break down barriers for SMBs🙌
            </div>
            
        </div>
        <div class="review">
            <div class="review-intro">
                <div class="customer-img">
                    <img src="../assets/customers/stephen.jpeg" alt="Customer">
                </div>
                <div class="customer-text">
                    <h4>Beng Aung</h4>
                    <p>Cheif Risk Officer, Sage</p>
                </div>
            </div>
            <div class="review-rating">
                ★★★★★
            </div>
            <div class="review-comment">
                Extremely rewarding collaborating with you <span>@Mass</span> and very much appreciate how you take our content, understand it and truly bring it to life, always with a striking and easily navigable UX⚡
            </div>
            
        </div>
        <div class="review">
            <div class="review-intro">
                <div class="customer-img">
                    <img src="../assets/customers/daniel.jpeg" alt="Customer">
                </div>
                <div class="customer-text">
                    <h4>Daniel Barnett</h4>
                    <p>Founder CEO, Worketc</p>
                </div>
            </div>
            <div class="review-rating">
                ★★★★★
            </div>
            <div class="review-comment">
                <span>@Mass</span> is without a doubt an attentive and talented designer, making him a reliable professional to work with. I would recommend him to anyone looking to step up their design game
            </div>
            
        </div>
        <div class="review">
            <div class="review-intro">
                <div class="customer-img">
                    <img src="../assets/customers/elana.jpeg" alt="Customer">
                </div>
                <div class="customer-text">
                    <h4>Elana Forde</h4>
                    <p>Talent Acquisition, Salt</p>
                </div>
            </div>
            <div class="review-rating">
                ★★★★★
            </div>
            <div class="review-comment">
                It was a pleasure working with <span>@Mass</span>, he is a highly skilled designer and the client only had amazing things to say. I would recommend him to anyone who is looking for an excellent designer and I hope to work with him again in the future!
            </div>
            
        </div>
        <div class="review">
            <div class="review-intro">
                <div class="customer-img">
                    <img src="../assets/customers/vee.jpeg" alt="Customer">
                </div>
                <div class="customer-text">
                    <h4>Vee Mercado</h4>
                    <p>Design Leader, WolliesX</p>
                </div>
            </div>
            <div class="review-rating">
                ★★★★★
            </div>
            <div class="review-comment">
                <span>@Mass</span> is visiually create and detailed, and has great eye for possiblities through understanding and sharing insights. Don't be surprised when you pick up a thing or two when collaborating with him
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
    .review-section {
        margin-top: 150px;
    }
    .review-h2 {
        font-size: 44px;
        font-weight: bold;
        margin-bottom: 18px;
    }
    .review-p {
        font-size: 22px;
        color: grey;
        margin-bottom: 42px;
    }

    .customer-review {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        /* background: red; */
        width: 1300px;
        margin: 0 auto;
    }
    .review {
        display: flex;
        flex-direction: column;
        flex: 0 0 25%;
        border: 1px solid rgb(218, 213, 213);
        box-shadow: 0 3px 0 0 rgb(218, 218, 218);
        border-radius: 15px;
        /* width: 320px; */
        padding: 24px;
        margin: 12px;
    }
    .review-intro {
        display: flex;
        align-items: center;
        margin-bottom: 6px;
    }
    .customer-img img{
        width: 70px;
        border-radius: 50%;
        margin-right: 12px;
    }
    .customer-text {
        /* background-color: red; */
        text-align: start;
    }
    .customer-text h4 {
        margin-bottom: -7px;
    }
    .review-rating {
        text-align: start;
        margin-bottom: 12px;
        color: #FDE272;
        font-size: 24px;
        font-weight: bold;
        letter-spacing: 4px;
    }
    .review-comment {
        text-align: start;
        line-height: 24px;
        font-size: 17px;
    }
    .review-comment span {
        color: rgb(71, 71, 226);
    }
</style>