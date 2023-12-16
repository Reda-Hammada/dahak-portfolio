<template>
  <section id="kontakt" class="w-[100%] mt-32">
    <h2 class="text-3xl ml-5 lg:ml-32 font-bold">Kontakt</h2>

    <div class="w-[90%] mt-12 mb-32 lg:ml-32">
      <div class="w-[100%] lg:w-[35%] mt-2 ml-5 text-xl">
        "Hi 👋" ,😊 Der schnellste Weg, mich zu erreichen, ist per E-Mail.
      </div>
      <div class="lg:w-[30%] w-[100%] mt-2 ml-5">
        <NuxtLink to="mailto:bewerbung@reda-dahak.de">
          <ReusableButton
            variant="  hover:bg-[#147efb] bg-black font-bold   text-white font-bold rounded   mt-5 w-[300px] h-[55px]  pr-[1%] pl-[1%]"
            text="bewerbung@reda-dahak.de"
          >
          </ReusableButton>
        </NuxtLink>
      </div>
    </div>
  </section>
</template>
