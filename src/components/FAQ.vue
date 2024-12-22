<template>
  <div class="faq">
    <div class="faq-span">FAQs</div>
    <div class="faq-h2">Frequently asked</div>
    <div class="faq-question-container" >
        <div class="faq-question" 
             @click="displayAnswer(item)" 
             v-for="item in checkFeild"
             :key="item.id"> 
            <div class="question-text">
                <h3>{{ item.title }}</h3>
                <span v-if="item.isVisible">-</span>
                <span v-else="item.isVisible">+</span>
            </div>
            <div class="question-answer" :class="{active: item.isVisible}">
                <p>
                    {{item.p}}
                </p>
            </div>
        </div>
    </div>
        
  </div>
</template>

<script>
export default {
    data() {
        return {
            checkFeild: [
            {id:1, title:'How do I get started?', p:'It’s simple. Choose a plan, click ‘Get started today’ and subscribe securely via Stripe. Within 24 hours you’ll receive a welcome email and the link to your personal Trello board, where you can submit your first design request right away. If this is your first time trying Artysan, you can opt for our 14-day plan as a one-time offer. After that, you can choose to continue with a monthly subscription.',  isVisible: false},
            {id:2, title:'Who will be working on my design?', p:'It’s simple. Choose a plan, click ‘Get started today’ and subscribe securely via Stripe. Within 24 hours you’ll receive a welcome email and the link to your personal Trello board, where you can submit your first design request right away. If this is your first time trying Artysan, you can opt for our 14-day plan as a one-time offer. After that, you can choose to continue with a monthly subscription.',  isVisible: false},
            {id:3, title:'How do I submit my requests?', p:'It’s simple. Choose a plan, click ‘Get started today’ and subscribe securely via Stripe. Within 24 hours you’ll receive a welcome email and the link to your personal Trello board, where you can submit your first design request right away. If this is your first time trying Artysan, you can opt for our 14-day plan as a one-time offer. After that, you can choose to continue with a monthly subscription.',  isVisible: false},
            {id:4, title:'How long does it take to receive my design?', p:'It’s simple. Choose a plan, click ‘Get started today’ and subscribe securely via Stripe. Within 24 hours you’ll receive a welcome email and the link to your personal Trello board, where you can submit your first design request right away. If this is your first time trying Artysan, you can opt for our 14-day plan as a one-time offer. After that, you can choose to continue with a monthly subscription.',  isVisible: false},
            {id:5, title:'How do I provide feedback for my designs?', p:'It’s simple. Choose a plan, click ‘Get started today’ and subscribe securely via Stripe. Within 24 hours you’ll receive a welcome email and the link to your personal Trello board, where you can submit your first design request right away. If this is your first time trying Artysan, you can opt for our 14-day plan as a one-time offer. After that, you can choose to continue with a monthly subscription.',  isVisible: false},
            {id:6, title:'Can I cancel or pause my subscription?', p:'It’s simple. Choose a plan, click ‘Get started today’ and subscribe securely via Stripe. Within 24 hours you’ll receive a welcome email and the link to your personal Trello board, where you can submit your first design request right away. If this is your first time trying Artysan, you can opt for our 14-day plan as a one-time offer. After that, you can choose to continue with a monthly subscription.',  isVisible: false},
            {id:7, title:'What software do you use for your work?', p:'It’s simple. Choose a plan, click ‘Get started today’ and subscribe securely via Stripe. Within 24 hours you’ll receive a welcome email and the link to your personal Trello board, where you can submit your first design request right away. If this is your first time trying Artysan, you can opt for our 14-day plan as a one-time offer. After that, you can choose to continue with a monthly subscription.',  isVisible: false}
            ]
            
        }
    },
    methods: {
        displayAnswer(item) {
           item.isVisible = !item.isVisible
           console.log('clicked');
        }
    }
}
</script>

<style>
    .faq {
        margin-top: 100px;
    }
    .faq-span {
        color: blue;
        font-size: 16px;
        font-weight: bold;
        margin-bottom: 22px;
    }
    .faq-h2 {
        font-size: 44px;
        font-weight: bold;
        margin-bottom: 62px;
    }
    .faq-question-container {
        margin: 12px;
    }
    .faq-question {
        display: flex;
        flex-direction: column;
        border: 1px solid grey;
        border-radius: 15px;
        width: 700px;
        margin: 16px auto;
        padding: 0px 32px;
        box-shadow: 1px 3px 0px 0px rgb(245, 244, 244);
    }
    .faq-question:hover {
        cursor: pointer;
        box-shadow: 1px 3px 1px 2px rgb(94, 93, 93);
        transition: all .3s;
    }
    .question-text {
        display: flex;
        align-items: center;
        justify-content: space-between;
        /* margin: -18px; */
        font-size: 16px;
    }
    .question-text span {
        font-size: 28px;
    }
    .question-answer {
        display: none;
        margin: 0;
        padding: 0;
        text-align: start;
        line-height: 20px;
        color: grey;
    }
    .question-answer.active {
        display: block;
    }
</style>