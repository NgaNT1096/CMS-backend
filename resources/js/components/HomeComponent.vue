<template>


        
          <div>
            <a>    <router-link :to="{ name: 'page' }">
                  List Page
                 </router-link></a>
               
                 <div>
                      <router-view></router-view>
                 </div>
         
          </div>
  

</template>

<script>
export default {
  name:"home-component",
  data (){
    return {
          title:0,
    }
  },
   methods: {



 
    ChangeTitle(){
    this.title++ ;
    },

 
  },

}
</script>>
<style scoped>
      @import url(https://fonts.googleapis.com/css?family=Dosis:300|Lato:300,400,600,700|Roboto+Condensed:300,700|Open+Sans+Condensed:300,600|Open+Sans:400,300,600,700|Maven+Pro:400,700);
      @import url("https://netdna.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.css");
      * {
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
        box-sizing: border-box;
      }
      header {
        color: #d3d3d3;
      }
      nav {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 82%;
        left: 0;
        padding: 22px;
        border-right: 2px solid #161e23;
      }
      nav > header {
        font-weight: 700;
        font-size: 0.8rem;
        text-transform: uppercase;
      }
      nav section {
        font-weight: 600;
      }
      nav section header {
        padding-top: 30px;
      }
      nav section ul {
        list-style: none;
        padding: 0px;
      }
      nav section ul a {
        color: white;
        text-decoration: none;
        font-weight: bold;
      }
      article {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        left: 18%;
        overflow: auto;
        border-left: 2px solid #2a3843;
        padding: 20px;
      }
      article > header {
        height: 60px;
        border-bottom: 1px solid #2a3843;
      }

</style>