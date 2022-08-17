<template>
  <div div class="container-fluid text-center bg-light">
    <!-- company logs container -->

    <Title
      mainTitle="OUR TEAM"
      subTitle1="Lorem ipsum dolor sit amet consectetur, adipisicing elit. In vitae inventore beatae."
      subTitle2="Exercitationem, nihil!"
    />

    <div class="row px-5 pb-3">
      <div class="col text-center my-1" :key="data.id" v-for="data in compData">
        <TeamComp :image="data.image" :name="data.name" :role="data.role" />
      </div>
    </div>

    <!-- blog snippets container -->
  </div>
</template>

<script>
import img2 from "~/assets/images/img2.jpeg"

export default {
  name: "Team",
  data() {
    return {
      compData: [
        {
          id: 1,
          image: img2,
          name: "Ramesh",
          role: "CEO",
        },
        {
          id: 2,
          image: img2,
          name: "Charlie",
          role: "CTO",
        },
        {
          id: 3,
          image: img2,
          name: "Atul",
          role: "Manager",
        },
        {
          id: 4,
          image: img2,
          name: "Arjun",
          role: "Designer",
        },
      ],
    };
  },
};
</script>