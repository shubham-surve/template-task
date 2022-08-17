<template>
  <div div class="container-fluid text-center bg-light p-0">
    <Title
      mainTitle="OUR PORTFOLIO"
      subTitle1="Lorem ipsum dolor sit amet consectetur, adipisicing elit. In vitae inventore beatae."
      subTitle2="Exercitationem, nihil!"
    />

    <div class="p-3 d-flex justify-content-center">
      <Button class="px-1" btnText="ALL" />
      <Button class="px-1" btnText="DESIGN" />
      <Button class="px-1" btnText="DEVELOPMENT" />
      <Button class="px-1" btnText="PRINT" />
    </div>

    <div class="row mx-5">
      <div
        class="col-4 justify-content-center p-2  "
        :key="data.id"
        v-for="data in compData"
      >
        <img class="img-fluid w-100" :src="data.image" alt="image" />
      </div>
    </div>

    <!-- VIDEO CONTAINER -->
    <div class="continer-fluid bg-secondary ">
      <Title
        mainTitle="WATCH OUR INTRO VIDEO"
        subTitle1="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eius."
        subTitle2="Tempor incididunt ut labore et dolore magna aliqua."
      />
      <div class="container-fluid text-center">
        <i class="p-5 fa-solid fa-circle-play fa-2xl"></i>
      </div>
    </div>
  </div>
</template>

<script>
import img1 from "@/assets/images/img1.jpeg";

export default {
  name: "Work",

  data() {
    return {
      compData: [
        { id: 1, image: img1 },
        { id: 2, image: img1 },
        { id: 3, image: img1 },
        { id: 4, image: img1 },
        { id: 5, image: img1 },
        { id: 6, image: img1 },
      ],
    };
  },
};
</script>
