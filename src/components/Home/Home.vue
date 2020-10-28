<template>
  <div class="">
    <section id="top" class="row">
      
      <kinesis-container class="numberFallContainer col-12 mx-auto row">
        <div class="container">
          <h1 class="col-12 my-5"><strong>{{ titre }}</strong></h1>
        </div>
        <div class="container mx-auto row">
        
          <article class="col-lg-6 mr-auto">
            <h2>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</h2>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat numquam facere eos placeat libero modi itaque voluptate? Reiciendis, at quam maxime, autem fuga, voluptatem vero iusto repellendus dolore modi perspiciatis voluptatum non ipsam dolorem consectetur dolores ut nisi.
            </p>      
          </article>
          <article class="viewport mx-auto row">            

                  <kinesis-element class="numberFallView"  :strength="-4">
                      <Numberfall style="font-size:20px;" class="mx-2"/>
                    </kinesis-element>

                  <kinesis-element class="numberFallView"  :strength="12">
                      <Numberfall style="font-size:12px;" class="mx-2"/>
                    </kinesis-element>

                  <kinesis-element class="numberFallView" :strength="-8">
                      <Numberfall style="font-size:22px;" class="mx-2"/>
                    </kinesis-element>

                  <kinesis-element class="numberFallView"  :strength="12">
                      <Numberfall style="font-size:12px;" class="mx-2"/>
                    </kinesis-element>

                  <kinesis-element class="numberFallView"  :strength="-4">
                      <Numberfall style="font-size:20px;" class="mx-2"/>
                    </kinesis-element>

                    <kinesis-element class="numberFallView"  :strength="8">
                      <Numberfall style="font-size:14px;" class="mx-2"/>
                    </kinesis-element>
                    
                    <kinesis-element class="numberFallView"  :strength="12">
                      <Numberfall style="font-size:12px;" class="mx-2"/>
                    </kinesis-element>

                    <kinesis-element class="numberFallView"  :strength="4">
                      <Numberfall style="font-size:16px;" class="mx-2"/>
                    </kinesis-element>
                    
                  <kinesis-element class="numberFallView"  :strength="12">
                      <Numberfall style="font-size:12px;" class="mx-2"/>
                    </kinesis-element>

                    <kinesis-element class="numberFallView"  :strength="0">
                      <Numberfall style="font-size:18px;" class="mx-2"/>
                    </kinesis-element>
                    
                    <kinesis-element class="numberFallView"  :strength="12">
                      <Numberfall style="font-size:12px;" class="mx-2"/>
                    </kinesis-element>


                      <div class="col-12 handContainer">
                        <!-- <kinesis-container> -->
                          
                            <kinesis-element  class="row" :strength="-20" axis="x">
                                <img class="col-6 mx-auto handView" src="../../assets/hand-planet.png" alt="">
                            </kinesis-element>
                            
                        <!-- </kinesis-container> -->
                    </div>

                    <kinesis-element class="numberFallView" :strength="-12">
                      <Numberfall style="font-size:24px;" class="mx-2"/>
                    </kinesis-element>

                  <kinesis-element class="numberFallView"  :strength="12">
                      <Numberfall style="font-size:12px;" class="mx-2"/>
                    </kinesis-element>

                    <kinesis-element class="numberFallView"  :strength="8">
                      <Numberfall style="font-size:14px;" class="mx-2"/>
                    </kinesis-element>

                    <kinesis-element class="numberFallView"  :strength="-4">
                      <Numberfall style="font-size:20px;" class="mx-2"/>
                    </kinesis-element>    

          </article>
        </div>
      </kinesis-container>
    </section>
    
    <kinesis-container class="row monolithSection my-5 py-5">
          <div class="monolithContainer container mx-auto row">
              <div class="col-6 monolithWrap">
                <kinesis-element  class="row" :strength="0" >
                    <!-- <img src="../../assets/mono-fond.png"> -->
                </kinesis-element>
              
                <kinesis-element  class="row shadowmonolith monolithImg" :strength="-20" axis="x" >
                  <img class="mx-auto" src="../../assets/mono-1-shadow.png" alt="">
                </kinesis-element>
                <kinesis-element  class="row jsutify-content-center monolith monolithImg" :strength="-30" >
                  <img class="mx-auto" src="../../assets/mono-1.png" alt="">
                </kinesis-element>
              
                <kinesis-element  class="row lightMonolith monolithImg" :strength="10" >
                    <img class="mx-auto" src="../../assets/mono-2.png" alt="">
                </kinesis-element>
                <kinesis-element  class="row shadowmonolith monolithImg" :strength="20" axis="x" >
                    <img class="mx-auto" src="../../assets/mono-2-shadow.png" alt="">
                </kinesis-element>

                <kinesis-element  class="row moveMediumMonolith monolithImg" :strength="30" >
                    <img class="mx-auto" src="../../assets/mono-3.png" alt="">
                </kinesis-element>
                <kinesis-element  class="row shadowmonolith monolithImg" :strength="40" axis="x" >
                    <img class="mx-auto" src="../../assets/mono-3-shadow.png" alt="">
                </kinesis-element>

                <kinesis-element  class="row veryLightMonolith monolithImg" :strength="50" >
                    <img class="mx-auto" src="../../assets/mono-4.png" alt="">
                </kinesis-element>
                <kinesis-element  class="row monolithImg shadowmonolith" :strength="60" axis="x" >
                    <img class="mx-auto" src="../../assets/mono-4-shadow.png" alt="">
                </kinesis-element>
              </div>

              <article class="col-lg-6 my-5 py-5">
                <h2>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</h2>
                <p>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat numquam facere eos placeat libero modi itaque voluptate? Reiciendis, at quam maxime, autem fuga, voluptatem vero iusto repellendus dolore modi perspiciatis voluptatum non ipsam dolorem consectetur dolores ut nisi.
                </p>        
              </article>
          </div>
    </kinesis-container>  
  </div>
  

</template>

<script>
  import Numberfall from './NumberFall'
  import { KinesisContainer, KinesisElement } from 'vue-kinesis';

    


  export default {
    
    name: 'Home',
    props: {},
    
    components: {
      Numberfall,
      'kinesis-container' : KinesisContainer,
      'kinesis-element' : KinesisElement
    },

    data(){
      return{
        titre: 'A la recherche d\'un développeur web ?!',
        dataForm: {
           item: '',
        },
        itemArray: ['Javascript', 'Vue', 'Python', 'React'],
        
      }
    },

    methods: {
      addItem: function(){
        this.itemArray.push(this.dataForm.item);
        this.dataForm.item = '';
      },
      removeItem: function(e){
        this.itemArray.splice(e.target.parentNode.id, 1)
      },


      

    },

  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped src="./Home.css">

</style>
