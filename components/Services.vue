<template>
  <div class="container-fluid text-center">
    <Title
      mainTitle="OUR SERVICES"
      subTitle1="Lorem ipsum dolor sit amet consectetur, adipisicing elit. In vitae inventore beatae."
      subTitle2="Exercitationem, nihil!"
    />

    <div class="px-5 row">
      <div class="p-5 col" :key="data.id" v-for="data in compData">
        <ServiceComp :img="data.image" :title="data.title" :para="data.para" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Services",
  data() {
    return {
      compData: [
        {
          id: 1,
          title: "Content Writing",
          para: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          image: '<i class="fa-solid fa-pen fa-2xl"></i>',
        },
        {
          id: 2,
          title: "Web Development",
          para: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          image: '<i class="fa-solid fa-code fa-2xl"></i>',
        },
        {
          id: 3,
          title: "Business Consultancy",
          para: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          image: '<i class="fa-solid fa-user-tie fa-2xl"></i>',
        },
      ],
    };
  },
};
</script>
