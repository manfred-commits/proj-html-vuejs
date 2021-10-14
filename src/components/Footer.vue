<template>
  <footer>
      <div class="page-margins">
          <div class="col-left">
              <img src="../assets/images/logo.png" alt="Brand logo footer">
              <div class="description-text-footer">
                  Ac aliquam neqwue sagittis diam faucibus vitae purus turpis phasellus. Pellentesque consectetur amet purus ultrices mauris.
              </div>
              <div class="social-links">
                <a class="social-link-formatting" v-for="(link,index) in footerData.footerLinksList" :key="link.name+index" :href="link.link">
                    <i :class="link.name"></i>
                </a>
                
              </div>
          </div>
          <div class="col-center">
              <h4>RECENT POSTS</h4>
              <ul>
                  <li v-for="(content,index) in footerData.recentPostsList" :key="content.content+index">
                      <a :href="content.link">
                        <h5>
                            <i class="fas fa-chevron-right"></i>
                            {{content.content}}
                        </h5>
                      </a>
                  </li>
              </ul>
          </div>
          <div class="col-right">
            <h5>CONTACTS INFORMATIONS</h5>
            <div class="contact-address">

                {{footerData.contactInfo.address}}
            </div>
            <div class="contact-phone">
                Mobile: {{footerData.contactInfo.mobilePhone}}
            </div>
            <div class="contact-email">
                Email: {{footerData.contactInfo.email}}
            </div>


          </div>
      </div>

      <section class="footer-bottom">
          ©Copyright 2012 - 2021 | Avada Theme by <a href="#">ThemeFusion</a>| All Rights Reserved | Powered by <a href="#">WordPress</a> 
      </section>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    props:['footerData'],
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables';


footer{
    background-color: $header_background_color;
    padding: 100px 0 0;
    color: $footer_primary_text_color;

    .page-margins{
        display: flex;
        align-items: flex-start;
        height: 100%;
        .col-left,
        .col-center,
        .col-right{
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            width: calc(100% / 3);

        }
        .col-left{
            font-size: 20px;
            img{
                margin: 30px 0;
                object-fit: cover;
                width: 50%;
                height: 100%;
            }
            .description-text-footer{
                text-align: center;
                color: $footer_secondary_text_color;
                width: 100%;
                padding-bottom: 50px;
            }
            .social-links{
                width: 100%;
                text-align: center;

                .social-link-formatting{
                    font-size: 20px;
                    color: $footer_icons_color;
                    margin: 0 10px;
                }
            }
        }
        .col-center{
            
            h4{
                font-size: 23px;
                width: 100%;
                text-align: center;
            }

            ul{
                list-style: none;
                margin: 40px 0;
                padding: 0;
                text-align: center;
                li{
                    padding: 10px;
                    a{
                        color: $footer_primary_text_color;
                        text-decoration: none;
                        h5{
                            font-size: 18px;
                        }
                    }
                }
            }
        }
        .col-right{
            font-size: 18px;

            h5,.contact-address,.contact-phone,.contact-email{
                text-align: center;
                width: 100%;
            }
            h5{
                font-size: 23px;
            }
            .contact-address{
                margin: 25px 0;
                color: $footer_secondary_text_color;
            }
        }
    }
    .footer-bottom{
        text-align: center;
        width: 100%;
        border-top: 1px solid rgb(70, 70, 70);
        color: $footer_secondary_text_color;
        font-size: 20px;
        padding: 60px 0;
        margin-top: 100px;

        a{
            text-decoration: none;
            color: $footer_primary_text_color;
        }
    }
}
</style>