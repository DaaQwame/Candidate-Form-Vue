<template>
  <form class="keep">
  <div class="slope">
    <input type="email" v-model="email" id="slip" class="loop" required name="email" placeholder="Enter Your Email Address">
    <br>
    <br>
    <div class="dope">
    <button @click="setPost" class="dim">Delete</button>
    </div>
  </div>
  </form>
<template/>
  
</template>
<script>
export default {
  data(){
    return { postData: { email: '' }}
  },
   methods: {
     setPost(event) {
      event.preventDefault()
      fetch('http://localhost:4000/api/candidates/delete', {
        method: 'DELETE',
        headers: {
          'Content-Type': 'application/json'
        },
        body: JSON.stringify({
          email: this.email
        })
      })
      .then(response => response.text())
      .then(data => console.log(data))
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
