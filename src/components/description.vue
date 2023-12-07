<script>
export default{
    name: "descrizione",
    data(){
        return{
           link:["characters","Comics","Movies","Tv","Games","Videos","News"]
        }
    },
}
</script>
<template>
   <div class="contenitorefooter">
     <div class="contenutofooter">
        <div>
            <h2>Dc Comics</h2>            
            <ul>
                <li v-for="links of link">
                    {{ links}}
                </li>
            </ul>
        </div>
        <div>

        </div>
        <div>

        </div>
     </div>
   </div>

</template>
<style lang="scss" scoped>
.contenitorefooter{
  background-image: url(../../public/img/img/footer-bg.jpg);
  .contenutofooter{
    width: 80%;
    margin: 0 auto;
  }
  li{
    list-style: none;
    color: #959595;
  }
  h2{
    color: white;
  }
}
</style>