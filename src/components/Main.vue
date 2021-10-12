<template>
  <main>

    <!-- fitness professional section -->
    <section class="fitnes-professional">
        <div class="page-margins section-formatting">
            <h4>Join our mailing list today</h4>
            <h2>Insider offers & flash sales in your inbox every week.</h2>

            <div class="fitness-hr">
                <i class="icon-formatting-left fas fa-chevron-up"></i>
                <i class="icon-formatting-center fas fa-chevron-up"></i>
                <i class="icon-formatting-right fas fa-chevron-up"></i>
            </div>

            <input type="text" placeholder="Insert your email...*">
            <button>Subscribe</button>

            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, consectetur adipiscing elit sed porttitor lectus.</p>
        </div>

    </section>


  </main>
</template>

<script>
export default {
    name: 'Main',
}
</script>

<style lang="scss" scoped>


.fitnes-professional{
    background-image:linear-gradient(90deg, rgba(0, 0, 1, 1)40%, rgba(0, 0, 1, 0.1) 60%),url('../assets/images/banner1-2x.jpg');    
    background-position: right;
    background-size: cover;
    background-repeat: no-repeat;

    
    .section-formatting{

        padding: 140px 0 350px;
        h4,h2,p{

            width: 50%;
        }

        h4{
            font-size: 30px;
            color: red;
        }
        h2{
            font-size: 60px;
            color: white;
        }
        p{
            color: grey;
            font-size: 28px;
        }
        

    }

}


</style>