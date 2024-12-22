<template>
  <div class="working-section">
    <div class="work-span">How it works</div>
    <div class="work-h2">The superpower of simplicity</div>
    <div class="work-p">Bringing you ideas to life has never been easier</div>

    <div class="work-feild">
        <div class="work-text">
            <div class="work-text-list" 
                v-for="item in workFeild" 
                :key="item.id"
                :class="{active: item.isActive}"
                @click="activeNow(item)">
                <h3>{{ item.title }}</h3>
                <p>{{ item.mainText }}</p>
            </div>
        </div>
        <div class="work-image">
            <img v-if="activeImage" :src="activeImage" alt="Active Image">
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            workFeild: [
                { id: 1, title: 'Subscribe and onboard', mainText: "Get started within minutes. choose your plan and subscribe via  Stripe. Welcome to Artysan", isActive: true, img: require('../assets/Working-imgs/Membership.png')},
                { id: 2, title: 'Request designs', mainText: "Use your personal Trello board to submit your design request. We'll get to work right away.", isActive: false, img: require('../assets/Working-imgs/Trello.png') },
                { id: 3, title: 'Subscribe and onboard', mainText: "Receive and review the design in Figma. Provide feedback and approve to finalise.", isActive: false, img: require('../assets/Working-imgs/Figma.png')}
            ],
            activeImage: require('../assets/Working-imgs/Membership.png')
        }
    },
    methods: {
        activeNow(clickedItem) {
            this.workFeild.forEach(item => {
            item.isActive = item.id === clickedItem.id;
            this.activeImage = clickedItem.img;
        });
        }
    }
}
</script>

<style>
    .working-section {
        display: flex;
        flex-direction: column;
        margin-top: 72px;
        padding-bottom: 72px;
        /* background-color: green; */
    }
    .work-span {
        color: #175CD3;
        font-weight: bolder;
        margin-bottom: 18px;
    }
    .work-h2 {
        font-size: 44px;
        font-weight: bolder;
        margin-bottom: 18px;
    }
    .work-p {
        font-size: 18px;
        color: #364A62;
        word-spacing: 1px;
        letter-spacing: 1px;
        margin-bottom: 74px;
    }
    .work-feild {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .work-text-list {
        border-left: 5px solid #ddd;
        /* background-color: red; */
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        width: 500px;
        padding-left: 16px;
        margin-bottom: 12px;
        color: rgb(206, 205, 205);
    }
    .work-text-list.active {
        color: black;
        border-left: 5px solid black;
    }
    .work-text-list.active:hover {
        color: black;
    }
    .work-text-list:hover {
        color: rgb(170, 166, 166);
        cursor: pointer;
    }
    .work-text-list h3 {
        margin-bottom: 12px;
    }
    .work-text-list p {
        margin: 0; 
        text-align: left; 
        letter-spacing: 1px;
        word-spacing: 1px;
    }
    .work-image img{
        width: 600px;
        margin-left: 59px;
    }
</style>