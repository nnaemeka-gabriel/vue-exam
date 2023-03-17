

<template>
   <div class="app">
	<Sidebar />
	<ToggleSwitch />
	
    <router-view />
    
	
   </div> 




 
</template>

<script setup>
  import Sidebar from './components/Sidebar.vue'  
import ToggleSwitch from './components/ToggleSwitch.vue'
  
</script>


<style lang="scss">
:root {

    --primary: #4a99de;
	--primary-alt: #22c55e;
	--grey: #64748b;
	--dark: #1e293b;
	--dark-alt: #334155;
	--light: #f1f5f9;
	--sidebar-width: 300px;
}
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Fira sans', sans-serif;
}
body {
	
background-image: url('./assets/jj.jpg');
	background-size: cover;
	
}
button {
	cursor: pointer;
	appearance: none;
	border: none;
	outline: none;
	background: none;
}

.app{
    display: flex;
    main {
        flex: 1 1 0;
        padding: 2rem;

       @media (max-width: 768px) {
          padding: 6rem;
       }  
    }
}

</style>