import { NuxtLink } from '../../.nuxt/components';
<template>
  <section id="zertifikats" class="w-[100%] mt-32">
    <h2 class="text-3xl ml-5 lg:ml-32 font-bold">Zertifikats</h2>
    <div
      class="w-[90%] ml-6 mt-16 mb-32 flex flex-col lg:flex-row justify-evenly"
      v-for="zertifikat in zertifikatS"
    >
      <div class="w-[100%] lg:w-[30%]">
        <h3 class="text-2xl font-bold">{{ zertifikat.title }}</h3>
        <div class="w-[100%] flex lg:hidden lg:w-[35%] mt-5">
          <NuxtImg
            class="rounded-lg"
            :src="`/images/${zertifikat.img}`"
            :alt="zertifikat.alt"
          />
        </div>
        <p class="mt-5 text-xl">{{ zertifikat.description }}</p>
        <NuxtLink target="_blank" :to="zertifikat.link">
          <ReusableButton
            variant="  hover:bg-[#147efb] bg-black  text-[16px] text-white font-bold rounded   mt-9 w-[150px] h-[40px]  pr-[1%] pl-[1%]"
            text="siehe Zertifikat"
          >
          </ReusableButton>
        </NuxtLink>
      </div>
      <div class="w-[100%] hidden lg:flex lg:w-[35%]">
        <NuxtImg
          class="rounded-lg"
          :src="`/images/${zertifikat.img}`"
          :alt="zertifikat.alt"
        />
      </div>
    </div>
  </section>
</template>
<script lang="ts" setup>
interface zertifikatsType {
  key: number;
  title: string;
  description: string;
  img: string;
  alt: string;
  link: string;
}

const zertifikatS: zertifikatsType[] = [
  {
    key: 1,
    title: "CCNAv7 : Einführung in Netzwerke",
    description:
      "Diese Zertifizierung kennzeichnet das grundlegende Verständnis für Netzwerkprinzipien, einschließlich Themen wie Netzwerkarchitektur, Protokolle und grundlegende Fehlerbehebung.",
    img: "netzwerk.png",
    alt: "netzwerk Reda Dahak netzwerktechniker certificate",
    link: "https://drive.google.com/file/d/1wN1N3fIW3Na28tX8qCdlr_NHZndWjUKg/view?pli=1",
  },
  {
    key: 2,
    title: "CCNAv7 : Switching - Routing- und Wireless-Grundlagen",
    description:
      "Kompetenz in grundlegenden Netzwerkfähigkeiten, insbesondere in den Bereichen Switching, Routing und drahtlose Technologien, durch die CCNAv7-Zertifizierung nachgewiesen.",
    img: "CNNA.png",
    alt: "Switching - Routing- und Wireless-Grundlagen Reda Dahak netzwerktechniker certificate",
    link: "https://drive.google.com/file/d/12283vtMTO4CKEdaZeb_kc96finaBTCvJ/view",
  },
  {
    key: 3,
    title: "CCNAv7 :Unternehmensnetzwerke ,Sicherheit und Automatisierung",
    description:
      "fortgeschrittene Wissen im Design und in der Absicherung von Unternehmensnetzwerken sowie  Expertise in der Implementierung von Automatisierung zur Verbesserung des Netzwerkmanagements und der Effizienz.",
    img: "cnnav7.png",
    alt: "Unternehmensnetzwerke ,Sicherheit und Automatisierung Reda Dahak netzwerktechniker certificate",
    link: "https://drive.google.com/file/d/1MWa6_gVPRHNzawUBGWFCBGYxX-o2J694/view",
  },
  {
    key: 4,
    title: "CISCO : Einführung in die Cybersicherheit",
    description:
      "grundlegendes Wissen in den Prinzipien der Cybersicherheit durch diese Cisco-Zertifizierung erworben, was sein Verständnis für wesentliche Konzepte und Praktiken zur Sicherung digitaler Umgebungen bestätigt.",
    img: "cyber.png",
    alt: "Einführung in die Cybersicherheit Reda Dahak netzwerktechniker certificate",
    link: "https://drive.google.com/file/d/11NpCOMz3vLzJr-BRY4J2iC4kKtD009up/view",
  },
  {
    key: 5,
    title: "Linux Essentials Professional Devlopment Certificate",
    description:
      "Linux-Betriebssystemen und umfasst grundlegende Fähigkeiten und Kenntnisse, die für effektive Systemadministration und Entwicklung in einer Linux-Umgebung erforderlich sind.",
    img: "ndg.png",
    alt: "Linux Essentials Reda Dahak netzwerktechniker certificate",
    link: "https://drive.google.com/file/d/10WO-X4dbJqQUFTyDL1M6NeZdnEfB1Mnb/view",
  },
  {
    key: 6,
    title: "Microsoft office specialist expert WORD und EXEL ",
    description:
      "Das Zertifikat für Microsoft Office Specialist Expert WORD und EXEL bestätigt fortgeschrittene Fähigkeiten und Kompetenzen im Umgang mit den weit verbreiteten Büroproduktivitätstools Word und Excel.",
    img: "moexpert.png",
    alt: "Microsoft office specialist expert WORD und EXEL Reda Dahak netzwerktechniker certificate",
    link: "https://drive.google.com/file/d/10Ywl2HsbRac1R3bZoHJJZueMLrvUAvaR/view",
  },
];
</script>
