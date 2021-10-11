<template>
  <main>

    <!-- fitness professional section -->
    <section class="fitnes-professional">
        <div class="page-margins section-formatting">
            <h4>Join our mailing list today</h4>
            <h2>Insider offers & flash sales in your inbox every week.</h2>

            <hr>

            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, consectetur adipiscing elit sed porttitor lectus.</p>
            <button>Visit my YouTube channel</button>
            <button>But Avada today</button>
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
    background-image:linear-gradient(to left, rgba(0, 0, 0,0), rgba(0, 0, 0,1) 62%),url('../assets/images/banner1-2x.jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;

    
    .section-formatting{

        padding: 140px 0 230px;
        h4{
            font-size: 30px;
            color: red;
        }
        h2{
            font-size: 60px;
            width: 80%;
            color: white;
        }

    }

}


</style>