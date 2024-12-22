<template>
    <!-- SPONSOR HTML -->
  <div class="sponsors">
    <div class="sponsor-span">
        Trusted by industry Leaders worldwide
    </div>
    <div class="sponsor-images">
        <img src="../assets/Sponsors/salt.svg" alt="salt image">
        <img src="../assets/Sponsors/opus.svg" alt="salt image">
        <img src="../assets/Sponsors/the-hundred.svg" alt="salt image">
        <img src="../assets/Sponsors/sage.svg" alt="salt image">
        <img src="../assets/Sponsors/major-league.svg" alt="salt image">
        <img src="../assets/Sponsors/ait.svg" alt="salt image">
        <img src="../assets/Sponsors/fitrli.svg" alt="salt image">
        <img src="../assets/Sponsors/work.svg" alt="salt image">
    </div>
  </div>

  <!-- BENEFITS HTML -->
   <div class="benefit-article">
        <div class="benefit-span">
            Benefits
        </div>
        <div class="benefit-h2">
            Out with the old, in with the <br> Awesome
        </div>
        <div class="benefit-p">
            Wave goodbye to costly traditional agencies and unreliable freelancers.
        </div>
        <div class="benefits-options">
            <div class="benefits-option">
                <img src="../assets/Benefits/flat-money.svg" alt="Flat Money Fee">
                <h3>Flat Monthly fee</h3>
                <p>Predictable budgeting with a fixed monthly <br> payment. No surprise, dead simple</p>
            </div>
            <div class="benefits-option">
                <img src="../assets/Benefits/revision.svg" alt="Flat Money Fee">
                <h3>Unlimited Revisions</h3>
                <p>We refine your design unitl you are fully <br> satisfied. Keep tweaking, it's on us. </p>
            </div>
            <div class="benefits-option">
                <img src="../assets/Benefits/turnaround.svg" alt="Flat Money Fee">
                <h3>Fast turnaround</h3>
                <p>Rapid delivery and updates every 48 hours. <br> The market moves fast, we move faster.</p>
            </div>
            <div class="benefits-option">
                <img src="../assets/Benefits/unique-design.svg" alt="Flat Money Fee">
                <h3>Unique professional design</h3>
                <p>Original designs that make your brand stand <br> out and shine. Boldly and beautifully.</p>
            </div>
            <div class="benefits-option">
                <img src="../assets/Benefits/no-locked-contract.svg" alt="Flat Money Fee">
                <h3>No locked contracts</h3>
                <p>Pause or cancel anytime, and come back <br> whenever. Full flexible, no headaches.</p>
            </div>
            <div class="benefits-option">
                <img src="../assets/Benefits/completely-async.svg" alt="Flat Money Fee">
                <h3>Completely async</h3>
                <p>Streamlined collaboration that respects your <br> time. Less meetings, more doings.</p>
            </div>
            
        </div>
   </div>
</template>

<script>
export default {

}
</script>

<style>
/* SPONSOR STYLING */
    .sponsors {
        margin-top: 65px;
    }
    .sponsor-span {
        font-size: 16px;
        word-spacing: 2px;
        margin-bottom: 11px;
    }
    .sponsor-images {
        display: flex;
        align-items: center;
        justify-content: center;
        margin-bottom: 122px;
    }
    .sponsor-images img{
        width: 100px;
        padding: 12px 25px;
        filter: brightness(3) saturate(0) invert(0) sepia(0.1);
    }
    .sponsor-images img:hover {
        cursor: pointer;
        filter: none;
        transition: all .1s;
    }
    .sponsor-images :first-child {
        width: 80px;
    }
    /* BENEFIT SYLING */
    .benefit-span {
        color: #175CD3;
        font-weight: bolder;
        font-size: 16px;
        margin-bottom: 18px;
    }
    .benefit-h2 {
        font-size: 36px;
        font-weight: bolder;
        margin-bottom: 16px;
    }
    .benefit-p {
        font-size: 19px;
        word-spacing: 1px;
        letter-spacing: 1px;
        color: #364A62;
    }
    .benefits-options {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        /* margin: 32px; */
        /* background: red; */
        margin: 0 auto;
        margin-top: 62px;
        width: 1300px;
    }
    .benefits-option {
        flex: 0 0 30%; 
        box-sizing: border-box; 
        margin: 5px; 
    }
    .benefits-option img {
        width: 140px;
    }
    .benefits-option p {
        line-height: 22px;
        font-size: 15px;
        color: #364152;
        
    }
</style>