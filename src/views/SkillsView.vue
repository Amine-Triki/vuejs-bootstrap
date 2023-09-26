<template>
    <main>
      <section class="Skills text-center pt-5 pb-5" id="Skills">
  <div class="container">
    <div class="main-title mt-5 mb-5 position-relative">
      <h2>My Skills</h2>
      <p>What I know</p>
    </div>
    <div class="Skill text-start ">
      <h3>HTML</h3>
      <div class="progress" role="progressbar"  aria-valuenow="80" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-success progress-bar-animated" style="width: 0" data-width="80%"></span>
      </div>
      <h3>CSS</h3>
      <div class="progress" role="progressbar"  aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-success progress-bar-animated" style="width: 0" data-width="75%"></span>
      </div>
      <h3>GIT</h3>
      <div class="progress" role="progressbar"  aria-valuenow="70" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-info progress-bar-animated" style="width: 0" data-width="70%"></span>
      </div>
      <h3>WORDPRESS</h3>
      <div class="progress" role="progressbar"  aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-info progress-bar-animated" style="width: 0" data-width="65%"></span>
      </div>
      <h3>JavaScript</h3>
      <div class="progress" role="progressbar"  aria-valuenow="62" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-info progress-bar-animated" style="width: 0" data-width="62%"></span>
      </div>
      <h3>SASS</h3>
      <div class="progress" role="progressbar"  aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-warning progress-bar-animated" style="width: 0" data-width="65%"></span>
      </div>
      <h3>BOOTSTRAP</h3>
      <div class="progress" role="progressbar"  aria-valuenow="55" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-warning progress-bar-animated" style="width: 0" data-width="55%"></span>
      </div>
      <h3>Adobe Photoshop</h3>
      <div class="progress" role="progressbar"  aria-valuenow="62" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-danger progress-bar-animated" style="width: 0" data-width="62%"></span>
      </div>
      <h3>Adobe xd</h3>
      <div class="progress" role="progressbar"  aria-valuenow="55" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-danger progress-bar-animated" style="width: 0" data-width="55%"></span>
      </div>
      <h3>Figma</h3>
      <div class="progress" role="progressbar"  aria-valuenow="57" aria-valuemin="0" aria-valuemax="100">
        <span class="progress-bar progress-bar-striped bg-danger progress-bar-animated" style="width: 0" data-width="57%"></span>
      </div>
    </div>
  </div>
  
</section> 
    </main>
</template>



<script>
export default {
    
    mounted(){
      let section = document.querySelector(".Skill");
let spans = document.querySelectorAll(".progress span");

window.onscroll = function () {
  if (window.scrollY >= section.offsetTop - 230) {
    spans.forEach((span) => {
      span.style.width = span.dataset.width;
    });
  }
};
}
}

</script>



<style>

/* start Skills*/
.main-title::after {
    content:"";
    width: 60px;
    height: 2px;
    background-color: #198754;
    position: absolute;
    bottom: -20px;
    left: 50%;
    transform: translateX(-50%);
    animation-name: ligne;
    animation-duration: 2s;
    animation-iteration-count: infinite;
}
/*  start keyframes */
@keyframes ligne {
    0% {
       transform-origin: right bottom;
    }
   
    25%{
        transform: rotateX(180deg);
    }
    75%{
        transform-origin: left bottom;
    }
    100%{
        transform: rotateZ(180deg);
    }
    
}
/* end keyframes */

.progress {
    position: relative;
    height: 20px;
    background-color: #fff;
    margin: 10px;
  }
  .progress span {
    position: absolute;
    left: 0;
    top: 0;
    height: 100%;
    background-color: #cd5c5c;
    transition: width 0.3s linear;
  }
/* end Skills*/


</style>