<template>
    <div>
            <article class="numberView mx-auto" v-for="(item, index) in vertiText" v-bind:key="index" v-html="item">
                  {{ item }}
            </article>
    </div> 
</template>

<script>
    export default {
        name: 'NumberFall',
        props: {},

        components:{

        },

        data(){
            return{
                vertiText: []
            }
        },

        methods:{

            moveArray:function(){
          
            var random2 = 1;
            //var i, randomLength;
            

            //randomLength = Math.floor(Math.random() * (0, 25) + 0);
          
            random2 = Math.floor(Math.random() * (0, 11));

             if(random2 == 10){
                 this.vertiText.unshift(' ' + '<br>')
             }else{
                this.vertiText.unshift(random2);
            }

            

            //  if( randomLength < 15 && randomLength > 10){
            //      for(i = 0; i < randomLength; i ++){
            //          this.vertiText.unshift(' ' + '<br>');
            //          console.log('heellooooo')
            //      }

            //  }

             if(this.vertiText.length == 30){
               this.vertiText.pop();
               
             }
             
            

             //console.log(this.vertiText.length)
            //console.log(random2);
            //console.log(this.vertiText.length);
            //console.log(this.itemArray);
            //setTimeout(this.moveArray(), 3000);
            
            //console.log(this.vertiText.length);
            //return this.vertiText;
            },
        
        launchMove: function(){
            //var random3 = Math.floor(Math.random() * (1000, 2000) + 0);
            //var toto = document.querySelectorAll('div.numberView');
            //console.log(random3);
            

            function getRandomIntInclusive(min, max) {
                min = Math.ceil(min);
                max = Math.floor(max);
                return Math.floor(Math.random() * (max - min +1)) + min;
            }
            var random3 = getRandomIntInclusive(300, 1400);
            console.log(random3);
            setInterval(function () { this.moveArray() }.bind(this), random3);
        }
    },

    mounted(){
      //this.getFall()
      this.launchMove()
    },
}

</script>

<style>
  

  .numberView{
    color: #2eff7e;
    text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 5px #00a130, 0 0 8px #00a130, 0 0 8px #00a130, 0 0 60px #00a130, 0 0 12px #00a130;
  }

</style>