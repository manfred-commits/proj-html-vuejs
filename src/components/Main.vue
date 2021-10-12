<template>
  <main>

    <!-- fitness list section -->
    <section class="fitnes-professional">
        <div class="page-margins section-formatting">
            <h4>Certified fitness professional</h4>
            <h2>Take control of your health</h2>

            <div class="fitness-hr">
                <i class="icon-formatting-left fas fa-chevron-up"></i>
                <i class="icon-formatting-center fas fa-chevron-up"></i>
                <i class="icon-formatting-right fas fa-chevron-up"></i>
            </div>

            <div class="description-text">
                Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet.
            </div>

            <button class="button-page">
                <i class="fab fa-youtube"></i>
                Visit my YouTube channel
            </button>

            <button class="button-page">
                Buy Avada today
                <i class="fas fa-arrow-right"></i>
            </button>
        </div>

    </section>
    <!-- /fitness list section -->


    <!-- mailing list section -->
    <section class="mailing-list">
        <div class="page-margins section-formatting">
            <h4>Join our mailing list today</h4>
            <h2>Insider offers & flash sales in your inbox every week.</h2>

            <div class="fitness-hr">
                <i class="icon-formatting-left fas fa-chevron-up"></i>
                <i class="icon-formatting-center fas fa-chevron-up"></i>
                <i class="icon-formatting-right fas fa-chevron-up"></i>
            </div>

            <input type="text" placeholder="Insert your email...*">
            <button class="button-page">Subscribe</button>

            <div class="description-text">
                Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, consectetur adipiscing elit sed porttitor lectus.
            </div>

        </div>

    </section>
    <!-- mailing list section -->




  </main>
</template>

<script>
export default {
    name: 'Main',
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables';


.fitnes-professional{
    background-image:linear-gradient(90deg, $header_background_color 47%, rgba(0, 0, 1, 0.1) 60%),url('../assets/images/slider82x-scaled.jpg');    
    background-position: top;
    background-size: cover;
    background-repeat: no-repeat;

    button{
        margin-left: 0;
    }
    

}
.mailing-list{
    background-image:linear-gradient(90deg, $header_background_color 47%, rgba(0, 0, 1, 0.1) 60%),url('../assets/images/banner1-2x.jpg');    
    background-position: right;
    background-size: cover;
    background-repeat: no-repeat;
    
}

.section-formatting{

    padding: 140px 0 280px;
    h4,h2,.description-text{
        width: 60%;
    }

    h4{
        font-size: 30px;
        color: $mailing_secondary_text_color;
    }
    h2{
        font-size: 80px;
        color: $mailing_primary_text_color;
    }
    .description-text{
        color: $mailing_description_text_color;
        font-size: 28px;
        margin-bottom: 50px;
    }
    

}

</style>