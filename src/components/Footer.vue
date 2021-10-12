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
                        <h5>{{content.content}}</h5>
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
                <strong>Mobile: {{footerData.contactInfo.mobilePhone}}</strong>
            </div>
            <div class="contact-email">
                <strong>Email: {{footerData.contactInfo.email}}</strong>
            </div>


          </div>
      </div>
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
    padding: 200px 0;
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
            font-size: 25px;
            img{
                margin: 30px 0;
                object-fit: cover;
                width: 50%;
                height: 100%;
            }
            .description-text-footer{
                text-align: center;
                width: 100%;
                padding-bottom: 50px;
            }
            .social-links{
                width: 100%;
                text-align: center;

                .social-link-formatting{
                    font-size: 25px;
                    color: $mailing_secondary_text_color;
                    margin: 0 10px;
                }


            }
        }
        .col-center{
            
        }
        .col-right{
            
        }
    }
}
</style>