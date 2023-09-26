<template>
  <main>
    <section class=" text-center pt-5 pb-5" id="Contact">
  <div class="container">
    <div class="main-title mt-5 mb-5 position-relative">
      <h2>Contact Me </h2>
      <p>Get in touch</p>
    </div>
    <div id="flex" class="d-flex  justify-content-center ">
      <div id="touch">
          <div class="text-start mt-4">
            <h3>
                Get in touch 
            </h3>
            <p class="mt-4">
                If you have any questions or proposals, you can simply write to us.<br> We will answer you as soon as possible.
            </p>
        </div>
        <div class="text-start d-flex justify-content-start align-items-center mt-4">
          <font-awesome-icon icon="fa-regular fa-user"  style=" margin-right: 10px;" />
            <div  class="head">
                <span><b>Name :</b></span>
                <span>Amine Triki</span>
            </div>
        </div>
        <div class="text-start d-flex justify-content-start align-items-center mt-4">
          <font-awesome-icon icon="fa-solid fa-location-dot" style=" margin-right: 10px;"/>
            <div class="head">
                <span><b>Address :</b></span>
                <span>Sakiet Ezzit , Sfax , Tunisia</span>
            </div>
        </div>
        <div class="text-start d-flex justify-content-start align-items-center mt-4">
          <font-awesome-icon icon="fa-regular fa-envelope" style=" margin-right: 10px;"/>
            <div  class="head">
                <span><b>Email :</b></span>
                <span>Contact@aminetriki.com.tn</span>
            </div>
        </div>
      </div>

      <form class="container mb-5 text-start mt-4" >
        <div class="row  mb-4">
          <div class="col">
            <label for="first-name">first name</label>
            <input type="text" class="form-control" id="first-name" placeholder="First name">
          </div>
          <div class="col">
            <label for="last-name">last name</label>
            <input type="text" class="form-control" id="last-name" placeholder="Last name">
          </div>
        </div>
        <div class="form-group mb-4">
            <label for="inputEmail4">Email</label>
            <input type="email" class="form-control" id="inputEmail4" placeholder="Email">
          </div>
        <div class="form-group mb-4">
          <label for="subject">subject </label>
          <input type="text" class="form-control" id="subject" placeholder="subject">
        </div>
        <button type="submit" class="btn btn-dark mb-4">Send</button>
      
      
      </form>

    </div>
  </div>
</section>
  </main>
</template>


<style>

/*  start contact */
form , #touch{ 
    flex: 1;
}
@media  (max-width: 992px) {
    #flex {
        flex-direction: column;
    }
}

/*end contact */

</style>