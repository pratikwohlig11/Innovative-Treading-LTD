<template>
  <div class="form">
    <div class="container">
      <div class="contact-form-data py-5 px-5 ">
        <h4 style="color: rgb(233, 69, 94); font-weight: 700">Contact Form</h4>
        <hr/>

        <div class="contact-form">
          <form class="text-start">
            <div class="mb-3">
              <label for="exampleInputEmail1" class="form-label">Name</label>
              <input
                type="name"
                class="form-control"
                id="exampleInputEmail1"
                aria-describedby="emailHelp"
              />
              <div id="emailHelp" class="form-text">
                We'll never share your email with anyone else.
              </div>
            </div>
            <div class="mb-3">
              <label for="exampleInputEmail1" class="form-label">Email</label>
              <input
                type="email"
                class="form-control"
                id="exampleInputEmail1"
                aria-describedby="emailHelp"
              />
              <div id="emailHelp" class="form-text">
                We'll never share your email with anyone else.
              </div>
            </div>
            <div class="mb-3">
              <label for="exampleInputEmail1" class="form-label"
                >Phone No:</label>
              <input
                type="number"
                class="form-control"
                id="exampleInputEmail1"
                aria-describedby="emailHelp"
              />
              <div id="emailHelp" class="form-text">
                We'll never share your email with anyone else.
              </div>
            </div>
            
            <h6>Message*</h6>
            <textarea
              name=""
              id=""
              style="width: 100%"
              cols="30"
              rows="10"
            ></textarea>

            <button type="submit" class="btn btn-primary">Submit</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.form{
    background-color: rgb(224,255,255)
}
</style>
