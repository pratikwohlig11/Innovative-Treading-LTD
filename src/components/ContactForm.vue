<template>
  <!-- <div>
    <div class="form">
      <div class="container">
        <h1>CONTACT US</h1>
        <div class="contact">
        <div>
          <label for="fname">Name:</label>
          <input type="text" v-model="Name" placeholder="Your Full name..." />
          <br><br>

          <label for="lname">Email:</label>
          <input
            type="text"
            v-model="Email"
            placeholder="Your Email Address..."
          />
          <br><br />
          <label for="fname">Phone No:</label>
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
  </div> -->
  <div>
    <div class="form">
      <div class="container">
        <h1>CONTACT US</h1>
        <div class="contact pb-5" style="margin: 0 150px;
          text-align: center;">
          <form class="text-center" @submit.prevent="getData">
            <div class="row">
              <div class="col-12" style="margin-bottom: 15px;">
                <div class="text-start mb-3">
                  <label></label>
                  <input
                    type="text"
                    class="form-control"
                    v-model.trim="$v.fullname.$model"
                    :class="{
                      'is-invalid': $v.fullname.$error,
                      'is-valid': !$v.fullname.$invalid,
                    }"
                    placeholder="Enter Your Full Name..."
                  />

                  <div class="valid-feedback">Your Full Name Is Valid</div>
                  <div class="invalid-feedback">
                    <span v-if="!$v.fullname.required"
                      >Your Full Name iS required.</span
                    >
                    <br />
                    <span v-if="!$v.fullname.minLength"
                      >Full Name Must Have At Least
                      {{ $v.fullname.$params.minLength.min }}letters</span
                    ><br />
                    <span v-if="$v.fullname.maxLength"
                      >Full Name Must Have At Most
                      {{ $v.fullname.$params.maxLength.max }}letters</span
                    >
                  </div>
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col-12">
                <div class="text-start mb-3">
                  <input
                    type="email"
                    @blur="$v.posts.email.$touch()"
                    class="form-control"
                    v-model.trim="$v.email.$model"
                    :class="{
                      'is-invalid': $v.email.$error,
                      'is-valid': !$v.email.$invalid,
                    }"
                    placeholder="Enter Your Email..."
                  />

                  <div class="valid-feedback">Your email Is Valid </div>
                  <div class="invalid-feedback">
                    <span v-if="!$v.email.required">Email is required.</span>
                    <br />
                   
                  </div>
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col-12" style="margin-bottom: 15px;">
                <div class="text-start mb-3" >
                  <label></label>
                  <input
                    type="number"
                    @blur="$v.posts.number.$touch()"
                    class="form-control"
                    v-model.trim="$v.phoneno.$model"
                    :class="{
                      'is-invalid': $v.phoneno.$error,
                      'is-valid': !$v.phoneno.$invalid,
                    }"
                    placeholder="Enter Your Phone No..."
                  />

                  <div class="valid-feedback">Your phone no Is Valid</div>
                  <div class="invalid-feedback">
                    <span v-if="!$v.phoneno.required"
                      >phoneno is required.</span
                    >
                    <br />
                    <span v-if="!$v.phoneno.isUnique"
                      >This phone No Is Already Registered
                      {{ $v.phoneno.$params.minLength.min }}numbers</span
                    ><br />
                    <span v-if="$v.phoneno.maxLength"
                      >Phone No Must Have At Most
                      {{ $v.phoneno.$params.maxLength.max }}numbers</span
                    >
                  </div>
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col-12">
                <div class="text-start mb-3">
                  <textarea
                    class="add"
                    @blur="$v.posts.address.$touch()"
                    name=""
                    v-model="address"
                    id=""
                    style="width: 100%"
                    cols="30"
                    rows="7"
                    placeholder="  Address..."
                  ></textarea>
                </div>
              </div>
            </div>

            <button class="btn btn-danger my-5">SUBMIT</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import {
  required,
  minLength,
  maxLength,
  email,
} from "vuelidate/lib/validators";
export default {
  name: "ContactForm",
  data() {
    return {
      // Name: "",
      // Email: "",
      // PhoneNo: "",
      // Address: "",
      fullname: "",
      email: "",
      phoneno: "",
      address:"",
    };
  },
  validations: {
    fullname: {
      required,
      minLength: minLength(6),
      maxLength: maxLength(10),
    },
    email: {
      email,
      required
      // isUnique(value) {
      //   if (value == "") return true;

      //   return new promise((resolve) => {
      //     setTimeout(() => {
      //       resolve(typeof value === "string" && value.length % 2 != 0);
      //     }, 350 + Math.random() * 300);
      //   });
      // },
    },
    phoneno: {
      required,
      minLength: minLength(10),
      maxLength: maxLength(10),
    },
     address: {
      required,
      minLength: minLength(30),
      maxLength: maxLength(50),
    },
  },

  methods: {
    getData() {
      console.log(this.fullname);
      console.log(this.email);
      console.log(this.phoneno);
      console.log(this.address);

      // this..reset();
    },
  },
};
</script>

<style scoped>
.form {
  background-color: rgb(224, 255, 255);
}

input {
  width: 100%;
  padding: 3px 0px 3px 10px;
  border-style: hidden;
}
h1 {
  padding-top: 30px;
  padding-bottom: 12px;
}
.add {
  border-style: hidden;
}
</style>
