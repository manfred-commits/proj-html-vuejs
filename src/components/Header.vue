<template>
  <header>
    <div class="page-margins">

        <div class="left-col">
            <img src="../assets/images/logo.png" alt="Brand logo header">
        </div> 

        <div class="right-col">

            <nav>
                <section id="page-navigation">
                    <ul>
                        <li v-for="(headerElement,index) in headerNavigationList" :key="headerElement.name+index">
                            <a :href="headerElement.link">
                                {{headerElement.name}}
                                <span v-if="headerElement.state==true" class="yellow-popup">new</span>
                            </a>
                        </li>
                    </ul>
                    <button class="button-header">Schedule a workout</button>
                    <i class="fas fa-shopping-cart icon-formatting"></i>
                    <i class="fas fa-search icon-formatting"></i>
                </section>


            </nav>

        </div>   


    </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    props:['headerNavigationList'],
    
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables';


header{
    background-color: $header_background_color;
    height: 13vh;
    color: $header_primary_text_color;
    font-size: 20px;


    .page-margins{

        @include header_components_verticalization;
        justify-content: space-between;
    
        .left-col{
            height: 100%;
            width: 18%;
            img{
                object-fit: contain;
                width: 100%;
                height:100%;
            }

        }

        .right-col{
            height: 100%;
            display: flex;
            align-items: center;
            flex-grow: 1;
            

            nav{

                @include header_components_verticalization;

                align-items: center;

                #page-navigation{

                    @include header_components_verticalization;
                    justify-content: flex-end;
                    
                    ul{
                        list-style: none;
                        display: flex;
                        flex-grow: 1;
                        justify-content: end;
                        align-items: center;
                        margin: 0;
                        
    
                        li{
                            margin: 0 15px;
                            
                            a{
                                text-decoration: none;
                                color: $header_primary_text_color;
                                font-size: 20px;
                            }
                            .yellow-popup{
                                display: inline-flex;
                                color: $primary_background_popup_color_text;
                                justify-content: center;
                                align-items: center;
                                background-color: $primary_background_popup_color;
                                padding: 5px;
                                border-radius: 5px;
                            }
                        }
                        :hover a {
                            color: $header_hover_primary_text_color;

                        }
                    }    
                    
                    .icon-formatting{
                        font-size: 20px;
                        margin: 5px 10px;
                        cursor: pointer;
                    }
                    .icon-formatting:hover{
                        color: $header_hover_primary_text_color;
                    }
                    .icon-formatting:last-child{
                        margin-right: 0;
                    }
                }
            }
            
        }

    }
}
</style>