<template>
  <div class="row">
    <add-product/>
    
    <contact-form/>

    <div class="p-3 col-7 text-font">
      <div class="card p-3 red-bg">
        <div class="row">
          <div class="card p-3 col-5 light-bg dashed-border">
          <p>Visit us at: Universitätsstraße 3, 79098 Freiburg im Breisgau, Germany.
          </p>
          <p>We're excited to meet you, so make sure you pull through, damnit!</p>
        </div>

        <div class="card col-7">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1099.514550716112!2d7.848087159633201!3d47.99488440172838!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47911c9ebee623eb%3A0xa1d69dc3344eb374!2sPuzzles!5e0!3m2!1sen!2sza!4v1692793756579!5m2!1sen!2sza" width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        </div>
        
      </div>

      <div class="pt-3 text-font">
        <div class="card p-3 yellow-bg">
          <h3>Alternatively, reach us at:</h3>
          <p>Email: <a href="mailto:taahirah.i@gmail.com">puzzlesdeli@unreal.net</a></p>
          <p>Mobile: <a href="tel:+0123456789">078 953 3354</a></p>
        </div>
      </div>
    </div>
  </div>

  <div class="p-3">
    <div class="row card p-3 red-bg"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import AddProduct from '@/components/AddProduct-Comp.vue'
import AddUser from '@/components/AddUser-Comp.vue'
import UpdateProduct from '@/components/UpdateProduct-comp.vue'
import ContactForm from '@/components/ContactForm-comp.vue'

export default {
  name: 'HomeView',
  components: {
    AddProduct,
    AddUser,
    UpdateProduct,
    ContactForm
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Lalezar&family=Londrina+Solid&display=swap");

.red-bg {
  background: #EE4823;
}

.yellow-bg {
  background: #F7BF3E;
}

.light-bg {
  background: #FAF9E8;
}

.dashed-border {
  border: 3px dashed #EE4823;
  border-radius: 10px;
}

.heading-font {
  font-family: "Lalezar", cursive;
}

.text-font {
  font-family: "Londrina Solid", cursive;
}
</style>