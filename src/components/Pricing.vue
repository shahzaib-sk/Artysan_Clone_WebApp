<template>
  <div class="pricing">
    <div class="pricing-span">Pricing</div>
    <div class="pricing-h2">Join Artysan today</div>
    <div class="pricing-p">Simple, predictable pricing. Choose your plan and start designing.</div>
    <div class="pricing-cards">
        <div class="starter-card">
            <div class="starter-span">Starter</div>
            <div class="starter-price">$1900 <span>/14 days</span></div>
            <div class="starter-p">First time? Try us out with a 14-day starter. <br>
                One-time offer for new customers.
            </div>
            <div class="starter-benefits">
                <ul>
                    <li>Dedicated Senior Designer</li>
                    <li>Full design services available</li>
                    <li>One request at a time</li>
                    <li>Delivery/updates every 48 hours</li>
                    <li>Unlimited requests/revisions</li>
                    <li>Unlimited brands/clients</li>
                    <li>Webflow development</li>
                </ul>
            </div>
            <div class="starter-btn"><button>Get started today</button></div>      
        </div>
        <div class="membership-card">
            <div class="starter-span">Membership</div>
            <div class="starter-price">$4000 <span>/month</span></div>
            <div class="starter-p">One monthly fee, endless possibilities. <br>
                Pause or cancel anytime.
            </div>
            <div class="starter-benefits">
                <ul>
                    <li>Dedicated Senior Designer</li>
                    <li>Full design services available</li>
                    <li>One request at a time</li>
                    <li>Delivery/updates every 48 hours</li>
                    <li>Unlimited requests/revisions</li>
                    <li>Unlimited brands/clients</li>
                    <li>Webflow development</li>
                </ul>
            </div>
            <div class="starter-btn">
                <button>Get started today</button>
            </div>      
        </div>
    </div>
    <div class="pricing-secure">🔒 Secure checkout via <span>stripe</span></div>
    <div class="contact">
        <div class="contact-img"><img src="../assets/person.png" alt="Person"></div>
        <div class="contact-text">
            <h3>Unsure? Book a Free intro call</h3>
            <p>Tell us about your projects, and let's find out if Artysan is right for you.</p>
        </div>
        <div class="contact-arrow">
            →	
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .pricing {
        margin-top: 95px;
    }
    .pricing-span {
        color: #175CD3;
        font-weight: bolder;
        margin-bottom: 18px;
    }
    .pricing-h2 {
        font-size: 48px;
        font-weight: bold;
        margin-bottom: 18px;
    }
    .pricing-p {
        font-size: 22px;
        word-spacing: 1px;
        color: grey;
        margin-bottom: 50px;
    }

    /* PRICING CARD STYLING */
    .pricing-cards {
        display: flex;
        justify-content: center;    
    }
    
    .starter-card {
        border: 3px solid rgb(204, 201, 201);
        border-radius: 15px;
        /* box-shadow: 10px 10px 15px -5px rgba(0, 0, 0, 0.2); */
        box-shadow: -4px 4px 0 3px rgb(224, 220, 220);
        width: max-content;
        padding: 44px;
        display: flex;
        flex-direction: column;
        text-align: start;
        margin: 21px;
    }
    .membership-card {
        border: 3px solid grey;
        border-radius: 15px;
        /* box-shadow: 10px 10px 15px -5px rgba(0, 0, 0, 0.2); */
        box-shadow: -4px 4px 0 3px rgb(37, 37, 37);
        width: max-content;
        padding: 44px;
        display: flex;
        flex-direction: column;
        text-align: start;
        margin: 21px;
    }
    .starter-span {
        font-size: 16px;
        font-weight: bolder;
        margin-bottom: 10px;
    }
    .starter-price {
        font-size: 32PX;
        font-weight: bold;
        margin-bottom: 10px;
    }
    .starter-price span {
        font-size: 20px;
        font-weight: 300;
    }
    .starter-p {
        color: grey;
        line-height: 20px;
        margin-bottom: 10px;
    }

    .starter-benefits{
        text-align: left;
        margin-bottom: 30px;
    }
    .starter-benefits ul{
        margin: 0;
        padding: 0;
    }
    .starter-benefits ul li {
        list-style-type: none;
        padding: 6px 0;
        color: black;
    }
    .starter-benefits ul li:before {
        content: '✓';
        color: blue;
        margin-right: 12px;
    }
    .starter-benefits ul li:nth-last-child(2) {
        color: grey;
    }
    .starter-benefits ul li:last-child {
        color: grey;
    }
    .starter-benefits ul li:last-child:before {
        content: '⦸';
        color: grey;
        /* margin-right: 12px; */
    }
    .starter-benefits ul li:nth-last-child(2):before {
        content: '⦸';
        color: grey;
        /* margin-left: 2px; */
        padding: 8px 0;
    }
    .membership-card:last-child ul li:last-child:before {
        content: '✓';
        color: blue;
        /* margin-right: 12px; */
    }
    .membership-card:last-child ul li:nth-last-child(2):before {
        content: '✓';
        color: blue;
        /* margin-left: 2px; */
    }
    .membership-card:last-child ul li:last-child {
        color: black;
    }
    .membership-card:last-child ul li:nth-last-child(2) {
        color: black;
    }
     .starter-btn {
        display: flex;
        justify-content: center;
        transition: all 0.3s;
    }
    .starter-btn button {
        padding: 18px 100px;
        color: white;
        font-weight: bold;
        font-size: 16px;
        border-radius: 15px;
        border: none;
        background: linear-gradient(to bottom, rgb(82, 80, 80), rgb(37, 37, 37));
        cursor: pointer;
    }
    .starter-btn button:hover {
        background: linear-gradient(to bottom, rgb(133, 131, 131), rgb(37, 37, 37));        
    }

    .pricing-secure {
        margin-top: 20px;
        margin-bottom: 35px;
        color: grey;
        font-size: 17px;
    }
    .pricing-secure span {
        color: blue;
        font-weight: bold;
    }
    .contact {
        display: flex;
        align-items: center;
        width: 500px;
        margin: 0 auto;
        padding: 18px 26px;
        border: 1px solid grey;
        border-radius: 16px;
        box-shadow: -4px 4px 0 3px rgb(224, 220, 220);
        transition: all .5s;
    }
    .contact-img img {
        border-radius: 50%;
        width: 100px;
    }
    .contact-text {
        width: 290px;
        margin: 0 auto;
    }
    .contact-arrow {
        font-size: 42px;
    }
    .contact:hover {
        cursor: pointer;
        box-shadow: -4px 4px 0 3px rgb(37, 37, 37);
    }
</style>