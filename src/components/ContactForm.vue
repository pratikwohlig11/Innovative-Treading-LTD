<template>
  <div>
    <div class="form">
      <div class="container">
        <h1>CONTACT US</h1>
        <div class="contact">
        <div>
          <!-- <label for="fname">Name:</label> -->
          <input type="text" v-model="Name" placeholder="Your Full name..." />
          <br><br>

          <!-- <label for="lname">Email:</label> -->
          <input
            type="text"
            v-model="Email"
            placeholder="Your Email Address..."
          />
          <br><br />
          <!-- <label for="fname">Phone No:</label> -->
          <input type="text" v-model="PhoneNo" placeholder="Phone No..." />
        </div>
          <br><br />
          <textarea class="add"
            name=""
            v-model="Address"
            id=""
            style="width: 31%"
            cols="30"
            rows="7"
            placeholder="Address..."
          ></textarea>
          
            <br /><br>
            <button v-on:click="SUBMIT">SUBMIT</button>
            <br><br>
        
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactForm",
  data() {
    return {
      Name: "",
      Email: "",
      PhoneNo: "",
      Address: "",
    };
  },
  methods: {
    SUBMIT() {
      console.log(this.Name, this.Email, this.PhoneNo, this.Address);
    },
  },
};
</script>

<style scoped>
.form {
  background-color: rgb(224, 255, 255);
}
.contact {
  /* width: 31%; */
/* padding: 3px 0px 3px 10px; */
}
input{
  width: 31%;
padding: 3px 0px 3px 10px;  
border-style: hidden;
}
h1{
    padding-top: 30px;
  padding-bottom: 12px;
}
.add{
  border-style: hidden;
}

</style>
