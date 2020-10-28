<template>
   <div>
    <b-navbar toggleable="lg">
    <b-navbar-brand href="#">NavBar</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#top">Accueil</b-nav-item>
        <b-nav-item href="#/Contact">Contact</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em>User</em>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
    </div>  
</template>

<script>
    export default {
        name: 'Navigation',
        data(){
          return{
            
          }
        }
    }
</script>

<style>
 div{
     color: #5c5c5c;
    

 }
</style>