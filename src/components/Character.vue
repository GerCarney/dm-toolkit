<template>
   <div class="character">

      <!-- Container -->
      <md-layout>

      <!-- Start left -->
      <md-layout class="left" md-flex-medium="70">
         <!-- First row -->
            <!-- Name Field -->
            <md-layout class="input-column" md-flex-medium="60">
               <md-input-container>
                  <label>Name</label>
                  <md-input v-model="name"></md-input>
               </md-input-container>
            </md-layout>

            <!-- Health Field -->
            <md-layout class="input-column" md-flex-medium="20">
               <md-input-container>
                  <label>Health</label>
                  <md-input type="number" v-model="health"></md-input>
               </md-input-container>
            </md-layout>

            <!-- AC Field -->
            <md-layout class="input-column" md-flex-medium="20">
               <md-input-container>
                  <label>AC</label>
                  <md-input type="number" v-model="ac"></md-input>
               </md-input-container>
            </md-layout>

         <!-- Second row -->
            <!-- Notes Field -->
            <md-layout class="input-column" md-flex-medium="100">
               <md-input-container md-clearable>
                  <label>Notes</label>
                  <md-textarea v-model="Notes"></md-textarea>
               </md-input-container>
            </md-layout>

            <!-- Third Row -->

            <!-- STR Field -->
            <md-layout class="input-column" md-flex-medium="20">
               <md-input-container>
                  <label>STR</label>
                  <md-input type="number" v-model="strength"></md-input>
               </md-input-container>
            </md-layout>

            <!--  DEX Field -->
            <md-layout class="input-column" md-flex-medium="20">
               <md-input-container>
                  <label>DEX</label>
                  <md-input type="number" v-model="dexterity"></md-input>
                  <span>+1</span>

               </md-input-container>
            </md-layout>

            <!-- WIS Field -->
            <md-layout class="input-column" md-flex-medium="20">
               <md-input-container>
                  <label>WIS</label>
                  <md-input type="number" v-model="wisdom"></md-input>
               </md-input-container>
            </md-layout>

            <!-- INT Field -->
            <md-layout class="input-column" md-flex-medium="20">
               <md-input-container>
                  <label>INT</label>
                  <md-input type="number" v-model="intelligence"></md-input>
               </md-input-container>
            </md-layout>

            <!-- CON Field -->
            <md-layout class="input-column" md-flex-medium="20">
               <md-input-container>
                  <label>CON</label>
                  <md-input type="number" v-model="constitution"></md-input>
               </md-input-container>
            </md-layout>


            <md-layout class="input-column" md-flex-medium="20">
               +1
            </md-layout>

            <md-layout class="input-column" md-flex-medium="20">
               +1
            </md-layout>

            <md-layout class="input-column" md-flex-medium="20">
               +1
            </md-layout>

            <md-layout class="input-column" md-flex-medium="20">
               +1
            </md-layout>

            <md-layout class="input-column" md-flex-medium="20">
               +1
            </md-layout>


      </md-layout>
      <!-- End left -->



      <md-layout class="right" md-flex-medium="30">

         <md-layout class="input-column" md-flex-medium="50">
               <label>Difficulty: 10</label>
         </md-layout>

         <md-layout class="input-column" md-flex-medium="50">
            <md-button class="md-fab">
              <md-icon>autorenew</md-icon>
            </md-button>
         </md-layout>



      </md-layout>
   </md-layout>



   </div>
</template>

<script>
export default {
   name: 'character',
   methods: {

   },
   data() {
      return {



      }
   },
   mounted() {

   }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.character {
   width: 96%;
   padding: 20px;
   box-shadow: 1px 1px 5px rgba(0,0,0,0.3);
   margin: 2%;
}

.input-column {
   padding: 0 10px;
}
</style>
