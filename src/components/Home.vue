<template>
    <main class='not-found'>
      <h1 class='heading-main'>Counter App</h1>
      <p class='home__msg'>Counter App with VueJS that performs Increment, decrement, Reset and set Value functions. 
      </p>
       
        <div class=btn_wrap> 
          <button type='button' class='btn'><router-link to="/counter">Counter</router-link> </button>
          <button type='button' class='btn'><a href='https://www.github.com/nnaemeka-gabriel'>GitHub</a> </button>
        </div>

        <span class='span'><p class='home__msg'> Designed with ❤️ and 💡 by Nnaemeka Gabriel</p></span>
    </main>
  </template>
  
  <script>
  export default {
    name: 'HomeApp'
  };
  </script>

<style>

.not-found{
    
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 20px;
  height: calc(100vh - 80px);
  width: 98%;
  margin: 0 auto;
  animation: fadeIn 1.5s ease-in-out;
  
}
.heading-main{
  font-size: 54px;
  margin-bottom: 16px;
  text-align: center;
  font-family: primaryFont;
  font-weight: bolder;
  color: var(--primary);
}
.home__msg{
  font-family: terFont;
  font-size: 18px;
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 20px;
  justify-content: center;
  align-items: center;
  color: var(--primary);
}

.btn_wrap .btn{

  width: 100px;
  height: 50px;
  outline: none;
  border: none;
  border-radius: 10px;
  margin: 10px;
  background-color: var(--light);
}
.btn a{
  text-decoration: none;
  font-weight: 600;
  font-size: 18px;
  font-family: primaryFont;
  color: var(--primary);
  

}
.btn a:hover{
    color: rgb(54, 113, 12);
}



@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>