<template>
  <div>
    <div class="form">
      <div class="container">
        <h1>CONTACT US</h1>
        <div class="contact pb-5" style="margin: 0 150px; text-align: center">
          <form class="text-center" @submit.prevent="getData" >
            


            <div class="row">
              <div class="col-12" style="margin-bottom: 15px">
                <div class="text-start mb-3">
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
                      >Your Full Name Is Required.</span>
                      <br>
                    <span v-if="!$v.fullname.onlytext"
                      >Alphabets Required.</span>
                  </div>
                </div>
              </div>
              
            </div>

            <div class="row">
              <div class="col-12">
                <div class="text-start mb-3">
                  <input
                    type="email"
                    class="form-control"
                    v-model.trim="$v.email.$model"
                    :class="{
                      'is-invalid': $v.email.$error,
                      'is-valid': !$v.email.$invalid,
                    }"
                    placeholder="Enter Your Email..."
                  />

                  <div class="valid-feedback">Your Email Is Valid</div>
                  <div class="invalid-feedback">
                    <span v-if="!$v.email.required">Email Is Required.</span>
                    <br />
                  </div> 
                </div>
               </div> 
            </div>

            <div class="row">
              <div class="col-12" style="margin-bottom: 15px">
                <div class="text-start mb-3">
                  <label></label>
                  <input
                    type="number"
                    class="form-control"
                    v-model.trim="$v.phoneno.$model"
                    :class="{
                      'is-invalid': $v.phoneno.$error,
                      'is-valid': !$v.phoneno.$invalid,
                    }"
                    placeholder="Enter Your Phone No..."
                  />

                  <div class="valid-feedback">Your Phone No Is Valid</div>
                  <div class="invalid-feedback">
                    <span v-if="!$v.phoneno.required"
                      >Numbers Is Required.</span
                    >
                    <br />
                    
                    
                    <br />
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
                    v-model.trim="$v.address.$model"
                    style="width: 100%"
                    cols="30"
                    rows="7"
                    placeholder="  Address..."
                  ></textarea>
                </div>
              </div>
            </div>

            <button class="btn btn-danger my-5" @click="getData()" input type="reset" value="reset" in>SUBMIT</button>















            
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
  alpha,
  helpers,
} from "vuelidate/lib/validators";

const onlytext = helpers.regex("onlytext", /^[a-zA-Z ]*$/);
// var regex = /^[a-zA-Z ]*$/;
export default {
  name: "ContactForm",
  data() {
    return {
      fullname: "",
      email: "",
      phoneno: "",
      address: "",
    };
  },
  validations: {
    fullname: {
      required,
      // minLength: minLength(0),
      // maxLength: maxLength(20),
      alpha,
      onlytext,
    },
    email: {
      email,
      required,
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
    reset: {},
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
  text-align: center;
}
.add {
  border-style: hidden;
}
@media only screen and (max-width: 576px) {
  .text-center {
    width: 100%;
  }
  .contact {
    margin: 0 !important;
  }
  .contact-data {
    padding: 0 !important;
  }
  .colr {
    word-wrap: anywhere;
  }
}
</style>
