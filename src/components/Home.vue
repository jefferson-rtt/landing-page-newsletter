<template>
  <div class="main">
    <div class="container">
      <h1 class="title">
        Subscribe to <strong>our Newsletter</strong>
      </h1>
      <p class="description">To get a discount on the first purchase and access to closed shares and sales.</p>
      <form class="form">
        <i class="fas fa-envelope"></i>
        <input type="email" required placeholder="Your Mail">
        <button type="submit" class="button">Subscribe</button>
      </form>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Home",
});
</script>

<style scoped>

.main{
  height: 100vh;
  background-color: #3161ff;
}

.container{
  height: 40%;
  width: 90%;
  max-width: 1150px;
  margin: 0 auto;
  display: grid;
  grid-auto-flow: row;
  grid-template-columns: auto;
  grid-template-rows: repeat(3, 1fr);
  align-items: center;
  justify-items: center;
  background-color: rgba(255, 255, 255, 0.146);
  border-radius: 12px;
  position: relative;
  top: 50%;
  transform: translateY(-50%);
  color: #f2f2f2;
  text-align: center;
}
.title{
  font-weight: 500;
}

.description{
  font-size: 1.2em;
}

.form{
  width: 50%;
  display: flex;
  justify-items: center;
  align-items: center;
  position: relative;
}

.form i{
  position: absolute;
  z-index: 10;
  color: #ffffff;
  left: 10px;
  
}
.form input{
  position: relative;
  height: 50px;
  width: 100%;
  padding: 0 90px 0 30px;
  background-color: #3a3a3a46;
  border-radius: 25px;
  border: none;
  outline: none;
  color: #f2f2f2;
  font-size: 1.125em;
}
.form input::placeholder{
  color: #f2f2f2;
  font-size: 1em;

}

.form button{
  position: absolute;
  right: 3px;
  width: auto;
  height: 80%;
  font-size: 1.125;
  border-radius: 25px;
  padding: 0 10px;
  background: #f2f2f2;
  color: #3161ff;
  border: none;
  font-weight: 700;
}

@media (max-width: 821px){
  .form{
    width: 90%;
  }
}

</style>
