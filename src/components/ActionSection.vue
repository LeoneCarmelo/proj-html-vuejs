<script>
export default {
    name: 'ActionSection'

}
</script>

<template>
      <section>
         <div class="container">
            <div class="row">
               <!-- Form -->
               <div class="col-8 pe-5">
                  <h6 class="color_dg fw-bold text-uppercase mb-3">send a message</h6>
                  <h3 class="fw-bolder mb-5">Get in<span class="bg_lg color_dg rounded-2 ms-2 px-2">Touch</span></h3>
                  <p class="text_grey">We will respond to your message as soon as possible.</p>
                  <form class="row g-3">
                     <div class="col-md-6">
                        <label for="inputName4" class="form-label"></label>
                        <input type="text" class="form-control border-0" id="inputName4" placeholder="Name">
                     </div>
                     <div class="col-md-6">
                        <label for="inputEmail4" class="form-label"></label>
                        <input type="email" class="form-control border-0" id="inputEmail4" placeholder="Email">
                     </div>
                     <div class="col-md-6 mt-0">
                        <label for="phone" class="form-label"></label>
                        <input type="text" class="form-control border-0" id="phone" placeholder="Phone">
                     </div>
                     <div class="col-md-6 mt-0">
                        <label for="inputInfo" class="form-label"></label>
                        <select id="inputInfo" class="form-select border-0">
                           <option>More Info</option>
                        </select>
                     </div>
                     <div class="col-12 mt-4">
                        <div class="message">
                           <textarea class="rounded-2 p-2 border-0" name="" id="" cols="59" rows="5"
                              placeholder="Message"></textarea>
                        </div>
                     </div>
                     <div class="col-12">
                        <button type="submit" class="btn bg_dg text-uppercase text-white">send</button>
                     </div>
                  </form>
               </div>
               <!-- Contacts -->
               <div class="col-4">
                  <h5 class="fw-bold">Example Inc.</h5>
                  <p class="text_grey">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  <p class="text_grey">Praesent diam lacus, dapibus sed imperdiet consectetur.</p>
                  <div class="contacts mt-4">
                     <div class="phone_number d-flex align-items-center">
                        <div class="icon">
                           <svg xmlns="http://www.w3.org/2000/svg" width="17" height="17" fill="currentColor"
                              class="bi bi-telephone-fill" viewBox="0 0 16 16">
                              <path fill-rule="evenodd"
                                 d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z" />
                           </svg>
                        </div>
                        <a href="#">+1 (305) 1234-5678</a>
                     </div>
                     <div class="contact_email d-flex align-items-center my-3">
                        <div class="icon">
                           <svg xmlns="http://www.w3.org/2000/svg" width="17" height="17" fill="currentColor"
                              class="bi bi-envelope-fill" viewBox="0 0 16 16">
                              <path
                                 d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z" />
                           </svg>
                        </div>
                        <a href="#">hello@example.com</a>
                     </div>
                     <div class="address d-flex align-items-center">
                        <div class="icon">
                           <svg xmlns="http://www.w3.org/2000/svg" width="17" height="17" fill="currentColor"
                              class="bi bi-geo-alt-fill" viewBox="0 0 16 16">
                              <path
                                 d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z" />
                           </svg>
                        </div>
                        <a href="#">Main Avenue, 987</a>
                     </div>
                     <button class="btn text-uppercase mx-2 color_dg my-4">view map</button>
                  </div>
               </div>
            </div>
         </div>
      </section>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
/* #region Utility */
.color_lg {
   color: $light-green
}

.color_dg {
   color: $dark-green
}

.bg_lg {
   background-color: $light-green;
}

.bg_dg {
   background-color: $dark-green;
}

.text_grey {
   color: $grey-text
}

/* #endregion Utility */
.container {
      width: 70%;
      padding: 6rem 0;

      input,
      select {
         background-color: $bg-input;
      }

      textarea {
         border: 1px solid rgb(209, 214, 219);
         resize: none;
         background-color: $bg-input;
      }

      .contacts a {
         text-decoration: none;
         padding:0 10px;
         color:$dark-green;
      }

      .icon {
         background-color: $light-green;
         width:35px;
         height:35px;
         border-radius: 50%;
         display: flex;
         justify-content: center;
         align-items: center;
      }

      .icon > svg {
         fill: $dark-green;
      }

      button {
         border: 1px solid $dark-green;
      }
   }

</style>