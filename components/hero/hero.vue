<template>
  <section
    id="heim"
    class="w-[100%] flex flex-col-reverse lg:flex-row justify-evenly flex-wrap lg:mt-[100px] mr-auto ml-auto"
  >
    <div class="w-[100%] lg:w-[40%]">
      <h1 class="text-3xl font-extrabold mt-28 text-center lg:text-start">
        Hallo 👋, ich bin Reda,ein
        <span class="text-[#147efb]">Netzwerktechniker</span>
      </h1>
      <p class="text-[20px] font-[400] mt-4 text-center lg:text-start">
        Ich bin ein Netzwerktechniker mit einer großen Leidenschaft für den IT-
        und Netzwerkbereich aus Marokko
      </p>
      <div class="lg:text-start text-center">
        <NuxtLink
          to="https://drive.google.com/uc?export=download&id=12nIcy_TvbUXo9DjyuOGeRxw9KmtWAu92"
        >
          <ReusableButton
            variant="  hover:bg-[#147efb] bg-black  text-[16px] text-white font-bold rounded   mt-9 w-[280px] h-[55px]  pr-[1%] pl-[1%]"
            text="Herunterladen meinen Lebenslauf"
          />
        </NuxtLink>
      </div>
      <div class="mt-5 text-center lg:text-start">
        <NuxtLink
          target="_blank"
          to="https://www.linkedin.com/authwall?trk=bf&trkInfo=AQGtYyx16jMxlgAAAYxGLdEoiUY5hlN83Foxkrkni5tkXT3NxGvn75bIHUkrSDL3dszCEfoDTtsBxvk9UbMZi51HIekiyzqQLvEhXm95gIrCwFvcSjG_CynvOBIdADkTsVKPt1c=&original_referer=&sessionRedirect=https%3A%2F%2Fwww.linkedin.com%2Fin%2Freda-dahak-a00bb5239%3Futm_source%3Dshare%26utm_campaign%3Dshare_via%26utm_content%3Dprofile%26utm_medium%3Dandroid_app"
        >
          <Icon name="uil:linkedin" color="#147efb" size="2em" />
        </NuxtLink>
      </div>
    </div>
    <div class="lg:w-[20%] w-[100%] mt-9 lg:mt-0 flex justify-center">
      <nuxt-img
        class="h-[500px] custom-border-radius"
        src="static/images/DSC_1869.jpg"
        alt=""
        loading="lazy"
      />
    </div>
  </section>
</template>
<script></script>
<style>
.custom-border-radius {
  border-radius: 30% 70% 77% 23% / 30% 34% 66% 70%;
}
</style>
