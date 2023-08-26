<template>
  <form class="keep">
  <div class="slope">
    <input type="email" v-model="email" id="slip" class="loop" required name="email" placeholder="Enter Your Email Address">
    <br>
    <br>
    <input type="password" v-model="password" id="slip" class="loop" required name="password" placeholder="Password">
    <br>
    <br>
    <div class="dope">
    <input type="submit" class="dim" value="Log In">
    </div>
  </div>
  </form>
<template/>
  
</template>
<script>
export default{
   data(){
    return{
      email: "",
      password: ""

       
    }
   }
}
</script>
<style>
.keep{
  display: flex;
  text-align: center;
  justify-content: center;
  margin-top: 10%;
}
.dim{
  padding: 15px;
  margin-left: 15%;
  background-color: rgb(248, 179, 52);
  color: #fff;
  font-weight: 500;
  font-size: 18px;
}
#slip{
  padding: 10px 35px;
}
.loop{
  border-radius: 5px;
  border: 2px solid #847d7d;
}
.slope{
  padding: 15px 100px 50px;
  box-sizing: border-box;
  box-shadow: 6px 10px 10px #888888;
}
</style>
