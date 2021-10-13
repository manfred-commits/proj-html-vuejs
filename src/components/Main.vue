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
        <div class="play-button">
            <a href="#" class="play-icon">
                <i class="fas fa-caret-right"></i>
            </a>
        </div>

    </section>
    <!-- /fitness list section -->


    <!-- endurance list section -->
    <section class="endurance-list">
        <div class="page-margins section-formatting">

            <div class="card-container">
                <!-- crossfit card -->
                <div class="basic-card">
                    <img src="../assets/images/service6-2x.jpg" alt="girl drinking">

                    <div class="hovering_box">

                        <div class="fitness-hr">
                            <i class="icon-formatting-left fas fa-chevron-up"></i>
                            <i class="icon-formatting-center fas fa-chevron-up"></i>
                            <i class="icon-formatting-right fas fa-chevron-up"></i>
                        </div>

                        <h3>Crossfit workout</h3>
                        <h5>Push your limits</h5>

                    </div>
                </div>
                <!-- /crossfit card -->

                <!-- crossfit card -->
                <div class="basic-card">
                    <img src="../assets/images/box1-2x.jpg" alt="girl drinking">

                    <div class="hovering_box">

                        <div class="fitness-hr">
                            <i class="icon-formatting-left fas fa-chevron-up"></i>
                            <i class="icon-formatting-center fas fa-chevron-up"></i>
                            <i class="icon-formatting-right fas fa-chevron-up"></i>
                        </div>

                        <h3>New gym apparel</h3>
                        <h5>Look good, feel good</h5>

                    </div>
                </div>
                <!-- /crossfit card -->

                <!-- crossfit card -->
                <div class="basic-card">
                    <img src="../assets/images/box3-2x.jpg" alt="girl drinking">

                    <div class="hovering_box">

                        <div class="fitness-hr">
                            <i class="icon-formatting-left fas fa-chevron-up"></i>
                            <i class="icon-formatting-center fas fa-chevron-up"></i>
                            <i class="icon-formatting-right fas fa-chevron-up"></i>
                        </div>

                        <h3>Team training</h3>
                        <h5>Find a partner</h5>

                    </div>
                </div>
                <!-- /crossfit card -->

            </div>
            
            <h2>"How you respond to the challenge in the second half will determine what you become after the game, whether you are a winner or a loser".</h2>

            <div class="fitness-hr">
                <i class="icon-formatting-left fas fa-chevron-up"></i>
                <i class="icon-formatting-center fas fa-chevron-up"></i>
                <i class="icon-formatting-right fas fa-chevron-up"></i>
            </div>

            <div class="testimanial-review">
                <img src="../assets/images/avatar-1-2x.jpg" alt="brad johnson photo">
                <h6>Brad Johnson</h6>
                <h6 class="location">Las Vegas</h6>
            </div>
            
            

        </div>

    </section>
    <!-- endurance list section -->   

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

    <!-- inspiration fail section -->
    <section class="inspirational-fail">
        <div class="page-margins section-formatting">
            <h2>"I've failed over and over again in my life. And that is why I succeed."</h2>

            <div class="inspirational-hr">
                <i class="icon-formatting-left fas fa-chevron-up"></i>
                <i class="icon-formatting-center fas fa-chevron-up"></i>
                <i class="icon-formatting-right fas fa-chevron-up"></i>
            </div>

            <div class="description-text">
                Arcu auctor gravida nisl, congue sit nisi tincidunt eget proin. In lacinia lacus donec sed massa in ipsum eros, tristique. Gravida suspendisse etiam in iaculis.
            </div>

            <button class="button-page">
                Buy Avada today 
                <i class="fas fa-chevron-right"></i>
            </button>


        </div>

    </section>
    <!-- inspiration fail section -->


  </main>
</template>

<script>
export default {
    name: 'Main',
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables';

.section-formatting{
    
    padding: 120px 0 120px;
    h4,h2,.description-text{
        width: 60%;
    }

    h4{
        font-size: 30px;
        color: $mailing_secondary_text_color;
    }
    h2{
        font-size: 70px;
        color: $mailing_primary_text_color;
    }
    .description-text{
        color: $mailing_description_text_color;
        font-size: 25px;
        margin-bottom: 50px;
    }
    
}

.fitnes-professional{
    background-image:linear-gradient(90deg, $header_background_color 47%, rgba(0, 0, 1, 0.1) 60%),url('../assets/images/slider82x-scaled.jpg');    
    background-position: top;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;

    button{
        margin-left: 0;
    }
}

.play-button{
    position: absolute;
    transform: translate(-50%,-50%);
    top: 50%;
    left: 80%;
    display: flex;
    color: black;
    width: 120px;
    height: 120px;
    background-color: white;
    border-radius: 50%;
    a{
        font-size: 50px;
        vertical-align: middle;
        margin: auto;
        text-decoration: none;
    }
}


.endurance-list{
    background-image: linear-gradient(to bottom right, blue , red);
    .section-formatting{
        text-align: center;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;

        .card-container{
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            position:relative;
            top: -180px;

            .basic-card{
                display: flex;
                box-shadow: 1px 2px 15px black;

                position: relative;
                width: calc(100% /3 - 80px);
                height: 500px;
                border-radius: 5px 5px 60px 0;
                overflow: hidden;

                img{
                    object-fit: cover;
                    width: 100%;
                }
                .hovering_box{
                   
                    position:absolute;
                    top: 0;
                    left: 0;
                    right: 0;
                    bottom: 0;
                    display: flex;
                    flex-wrap: wrap;
                    align-content: flex-end;
                    background-image:linear-gradient(360deg, $header_background_color -5%, rgba(0, 0, 1, 0.1) 60%);  

                    h3,h5{
                        text-align: left;
                        margin-left: 10%;
                    }

                    h3{
                        color: white;
                        width: 100%;
                        font-size: 35px;
                    }
                    h5{
                        color: yellow;
                        width: 100%;
                        font-size: 25px;

                        margin-bottom: 15%;

                    }

                    .fitness-hr{
                        height: 40px;
                        .icon-formatting-left,
                        .icon-formatting-center,
                        .icon-formatting-right{
                            font-size: 20px;
                            color: white;
                        }
                        .icon-formatting-left{
                            left:53px;
                        }
                        .icon-formatting-center{
                            left: calc(53px + 14px);
                        }
                        .icon-formatting-right{
                            left: calc(106px - 25px);
                            
                        }
                    }
                }

            }
        }

        h2{
            width: 80%;
            font-size: 50px;
        }
        .fitness-hr{
            width: 100%;
            position: relative;
            .icon-formatting-left,
            .icon-formatting-center,
            .icon-formatting-right{
                position: absolute;
                color: $yellor_page_color;
                font-size: 30px;
                top: 50%;
                
            }
            .icon-formatting-left{
                left:calc(50% + -22px);
            }
            .icon-formatting-center{
                left: 50%;
            }
            .icon-formatting-right{
                left: calc(50% + 20px);
                
            }
        }
        .testimanial-review{
            display: flex;
            align-items: center;
            img{
                border-radius: 50%;
                object-fit: contain;
                height: 60px;
            }
            h6{
                font-size: 20px;
                padding: 0 15px;
                color: white;
            }
            .location{
                font-weight: 400;
                color: lightgrey;
                padding-left: 0;
            }
        }
    }

}


.mailing-list{
    background-image:linear-gradient(90deg, $header_background_color 47%, rgba(0, 0, 1, 0.1) 60%),url('../assets/images/banner1-2x.jpg');    
    background-position: right;
    background-size: cover;
    background-repeat: no-repeat;
    
}

.inspirational-fail{
    background-image:linear-gradient(360deg, $header_background_color 5%, rgba(23, 23, 170, 0.1) 60%),url('../assets/images/banner2-2x.jpg');    
    background-position: center top;
    background-size: cover;
    background-repeat: no-repeat;

    .section-formatting{
        text-align: center;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        padding: 240px 0 100px;

        h4,h2,.description-text{
        width: 70%;
        margin: auto;
        }    

        // custom hr for section
        .inspirational-hr{
            padding: 50px 0;
            margin-bottom: 50px;
            width: 100%;
            position: relative;

            .icon-formatting-left,
            .icon-formatting-center,
            .icon-formatting-right{
                position: absolute;
                color: $yellor_page_color;
                font-size: 30px;
                top: 50%;
                
            }
            .icon-formatting-left{
                left:calc(50% + -34px);
            }
            .icon-formatting-center{
                left:calc(50% + -13px);

            }
            .icon-formatting-right{
                left: calc(50% + 8px);
                
            }
        }    
        .description-text{            
            color: $mailing_primary_text_color;
            font-size: 25px;
        }
        .button-page{
            margin: 50px 150px;
        }
    }
}



</style>