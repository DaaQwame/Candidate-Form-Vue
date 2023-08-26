<template>
  <form id="flip">
    <div id="play">
      <header>
  <h1>ONLINE VOTING SYSTEM</h1>
  </header><hr>
  <div class="down">
      <h3>REGISTRATION</h3>
      </div>
    <label>Full Name</label>
    <input type="text" id="one" v-model="full_name" name="full name" required placeholder="Enter Your Full Name"><br>
    <label>Place Of Birth</label>
    <input type="text" id="one" v-model="place_of_birth" name="place of birth" required placeholder="Enter Place Of Birth"><br>
    <label>Gender</label>
    <input type="text" id="one" v-model="gender" name="gender" required placeholder="Enter Your Gender"><br>
    <label>Email</label>
    <input type="email" id="one" v-model="email" name="email" required placeholder="Enter Your Email"><br>
    <label>Phone Number</label>
    <input type="text" id="one" v-model="phone_number" name="phone number" required placeholder="Enter Your Phone Number"><br>
    <label>Date Of Birth</label>
    <input type="date" id="one" v-model="date_of_birth" name="date of birth" required placeholder=" Enter Your Date Of Birth"><br>
    <label>ID Type</label>
    <input type="text" id="one" v-model="id_type" name="id type" required placeholder="Enter ID Type"><br>
    <label>ID Number</label>
    <input type="text" id="one" v-model="id_number" name="id number" required placeholder="Enter ID Number"><br>
    <label>Password</label>
    <input type="password" id="one" v-model="password" name="password" required placeholder="Enter Your Password"><br>
    <div class="leak">
    <input type="submit" class="soso" value="Submit" >
    </div>
    </div>
  </form>
</template>

<script>
export default {
  data(){
    return{
      full_name: "",
      place_of_birth: "",
      gender: "",
      email: "",
      phone_number: "",
      date_of_birth: "",
      id_type: "",
      id_number: "",
      password: ""
    }
  }
}
</script>

<style>
span{
  padding-left: 50px;
}
#flip{
  display: flex;
  align-items: center;
  justify-content: center;
}
#flip #play{
  padding: 30px 40px;
  box-sizing: border-box;
  box-shadow: 4px 10px 15px #888888;
}
.leak{
  padding: 10px;
  width: 100%;
}

.soso{
  padding: 10px;
  background-color: rgb(248, 179, 52);
  color: #fff;
  font-weight: 500;
  font-size: 18px;
}
.down{
  display: flex;
  align-items: center;
  justify-content: center;
}
label{
  padding-right: 10px;
  margin-top: 40%;
}
input{
  width: 90%;
  border-radius: 5px;
  border: 2px solid #847d7d;
  height: 20%;
}
#one{
   padding: 10px;
}

</style>
