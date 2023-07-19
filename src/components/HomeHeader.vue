<script setup>
import gsap from "gsap";
import { onMounted } from "vue";

onMounted(() => {
  gsap
    .timeline()
    .to(".letter", {
      duration: 0.3,
      scale: 1,
      fontSize: "3rem",
      stagger: 0.2,
      ease: "elactic",
    })
    .to(".message", {
      opacity: 1,
      y: 0,
      duration: 1,
      ease: "back.out(1.7)",
    })
    .to(".talk-wrapper", {
      opacity: 1,
      y: 0,
      duration: 1,
      ease: "back.out(1.7)",
    });
});
</script>

<template>
  <header class="md:flex mt-10">
    <div class="md:flex-1">
      <div class="text-center md:text-left">
        <div
          class="callout top-right inline-block bg-kjColorDark text-kjColorLight shadow"
          style="transform: translate(0px, 0px)"
        >
          Hola Soy,
        </div>
        <h1 class="text-5xl font-black leading-none mb-4">
          <span class="letter">J</span><span class="letter">o</span
          ><span class="letter">h</span><span class="letter">a</span>
          <span class="letter">n</span> <span class="letter">H</span
          ><span class="letter">.</span> <br /><span class="letter">F</span
          ><span class="letter">a</span><span class="letter">c</span
          ><span class="letter">u</span>
          <span class="letter">n</span>
          <span class="letter">d</span>
          <span class="letter">o</span>
        </h1>
      </div>
      <p
        class="text-kjColorGray text-sm mt-10 text-center md:text-left px-5 md:px-0 md:w-64 message"
        style="/*transform: translate(0px, 0px); opacity: 1*/"
      >
        Un desarrollador de software enfocado en la construcción de sistemas a
        me medida.
      </p>

      <div class="mt-10 talk-wrapper">
        <a href="mailto:E.Johan.Herrera.F@Gmail.com" target="_blank">
          <div class="talk">
            <div class="talk2">contact me</div>
            <div class="talk-pulse"></div>
          </div>
        </a>
      </div>

      <!-- <div class="mt-10 talk-wrapper" style="opacity: 1">
              <a href="mailto:E.Johan.Herrera.F@Gmail.com" target="_blank">
                <div class="talk" style="transform: translate(0px, 0px)">
                  <div class="talk2">contact me</div>
                  <div
                    class="talk-pulse"
                    style="opacity: 0; transform: scale(3, 3)"
                  ></div>
                </div>
              </a>
            </div> -->
    </div>
    <div class="mt-10 md:flex-1">
      <img
        src="@/assets/profile_Caricature2.webp"
        alt="Johan photo"
        class="wr-19 ml-auto mr-auto md:ml-0 md:mr-0 md:w-128"
      />
    </div>
  </header>
</template>
<style>
.talk-wrapper {
  position: relative;
  opacity: 0;
  transform: translateY(100px);
}

.talk {
  position: relative;
  right: -55px;
  z-index: 2;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 15px solid hsla(7, 76%, 69%, 0.863);
  background: #d64633;
  border-radius: 50%;
  height: 100px;
  width: 100px;
  text-align: center;
  font-weight: 600;
  color: white;
}

.callout.top-right:before {
  right: 7px;
  bottom: -20px;
  border-top: 10px solid #2b2929;
}

.callout:before {
  content: "";
  width: 0;
  height: 0;
  border: 0.8em solid transparent;
  position: absolute;
}

.callout {
  height: 18px;
  width: 90px;
  background-image: -moz-linear-gradient(top, #2b2929, #2b2929);
  position: relative;
  padding: 10px;
  border-radius: 3px;
  margin: 25px;
  min-height: 50px;
  border: 1px solid #2b2929;
  text-shadow: 0 0 1px #000;
  transform: scale(0);
}
</style>
