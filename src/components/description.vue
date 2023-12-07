<script>
import pagefoot from './pagefoot.vue';

export default{
    name: "descrizione",
    data(){
        return{
           link:["characters","Comics","Movies","Tv","Games","Videos","News"],
           dc:["Terms of use","Privacy Policy (New)","Ad Choices","Advertising",
          "Jobs","Subscriptions","Talent Workshops","CPSC Certificates","Ratings","Shop Help","Contact Us"],
          shop:["Shop DC","Shop DC Collectibles"],
          sites:["DC","MAD Magazine","DC Kids","DC Universe","DC Power Visa"],
        }
    },
    components:{
      pagefoot,
    }
}
</script>
<template>
   <div class="contenitorefooter">
     <div class="contenutofooter">
        <div class="contenitorelink">
            <h2>Dc Comics</h2>            
            <ul>
                <li v-for="links of link">
                    {{ links}}
                </li>
            </ul>
            <h2>Shop</h2>
            <ul>
              <li v-for=" shops in shop">
                {{ shops }}
              </li>
            </ul>
        </div>
        <div class="contenitorelink">
            <h2>DC</h2>
            <ul>
              <li v-for="dcs in dc">
                 {{ dcs }}
              </li>
            </ul>
        </div>
        <div class="contenitorelink">
          <h2>Site</h2>
          <ul>
            <li v-for="site in sites">
              {{ site }}
            </li>
          </ul>
        </div>
        <div class="contenitoreimg">
           <img src="../../public/img/img/dc-logo-bg.png" alt="logo">
        </div>
     </div>
   </div>
   <div>
    <pagefoot></pagefoot>
   </div>

</template>
<style lang="scss" scoped>
.contenitorefooter{
  background-image: url(../../public/img/img/footer-bg.jpg);
  .contenutofooter{
    width: 80%;
    margin: 0 auto;
    display: flex;
    position: relative;
    padding-bottom: 55px;
  }
  li{
    list-style: none;
    color: #959595;
    margin-bottom: 10px;
    font-size: 14px;
  }
  h2{
    color: white;
    margin-bottom: 20px;
  }
  .contenitorelink{
    margin-top: 40px;
    margin-right: 50px;
  }
  .contenitoreimg{
    position: absolute;
    top: -60px;
    right: 0px;
  }
}
// .hello{
//    position: relative;
//    .hello2{
//     position: absolute;
//     background-color: black;
//     height: 200px;
//     width: 100%;
//    }
//   }

</style>