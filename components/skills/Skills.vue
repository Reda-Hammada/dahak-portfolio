<template>
  <section id="skills" class="w-[100%] mt-32">
    <h2 class="text-3xl ml-5 lg:ml-32 font-bold">Fähigkeiten</h2>
    <div
      class="flex lg:ml-32 flex-wrap justify-start w-[100%] lg:justify-start"
    >
      <div class="mt-7" v-for="skill in skillsIcons">
        <NuxtImg
          :src="skill.src"
          :alt="skill.alt"
          :key="skill.key"
          loading="lazy"
          class="w-[140px] text-center h-[145px] ml-7 lg:ml-9 border-none rounded-md bg-white"
        />
      </div>
    </div>
  </section>
</template>
<script lang="ts" setup>
interface skillsTypes {
  key: number;
  src: string;
  alt: string;
}

const skillsIcons: skillsTypes[] = [
  {
    key: 1,
    src: "../../images/ccna.png",
    alt: "ccna skill",
  },
  {
    key: 2,
    src: "../../images/ws.png",
    alt: "window server",
  },

  {
    key: 3,
    src: "../../images/linux.png",
    alt: "linux ",
  },
  {
    key: 4,
    src: "../../images/vmware.jpg",
    alt: "vmware ",
  },

  { key: 5, src: "../../images/vbox.png", alt: "virtual box " },
  { key: 6, src: "../../images/python.png", alt: "Python  " },
  { key: 7, src: "../../images/moffice.png", alt: "moffice  " },
];
</script>
