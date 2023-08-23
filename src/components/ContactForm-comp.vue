<template>
  <div class="p-3 col-5">
    <form
      action="https://formspree.io/f/mzblrvgp"
      method="POST"
      class="card p-3 green-bg"
    >
      <div class="mb-3 text-font">
        <label for="fullName" class="form-label">Full Name(s): *</label>
        <input
          v-model="fullName"
          type="text"
          id="fullName"
          name="Full Name"
          class="form-control input-bg"
          placeholder="eg: Clayton Margaret Sherman"
          required
        />
      </div>

      <div class="mb-3 text-font">
        <label for="email" class="form-label">Email: *</label>
        <input
          v-model="email"
          type="text"
          id="email"
          name="Email"
          class="form-control input-bg"
          placeholder="eg: claytonmsherman@hotmail.com"
          required
        />
      </div>

      <div class="mb-3 text-font">
        <label for="message" class="form-label">Message:</label>
        <textarea
          v-model="message"
          id="message"
          name="Message"
          class="form-control"
          rows="5"
          placeholder="Leave us a message and we'll get back to you soon!"
        ></textarea>
      </div>

      <p class="text-font">* indicates a required field.</p>

      <div class="p-3 text-center">
        <button type="submit" class="btn m-2 add-btn text-font">
          Submit!
        </button>
        <button type="reset" class="btn m-2 clr-btn text-font">
          Clear Fields
        </button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fullName: "",
      email: "",
      message: "",
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Lalezar&family=Londrina+Solid&display=swap");
.green-bg {
  background: #45a245;
}

.input-bg {
  background: #faf9e8;
}

.heading-font {
  font-family: "Lalezar", cursive;
}

.text-font {
  font-family: "Londrina Solid", cursive;
}

.add-btn,
.clr-btn {
  border: 3px solid #ee4823;
  border-radius: 20px;
  background: #faf9e8;
  width: 45%;
}
</style>
