<template>
  <div class="container-fluid text-center bg-secondary">
    <Title
      mainTitle="SOME FEATURES"
      subTitle1="Lorem ipsum dolor sit amet consectetur, adipisicing elit. In vitae inventore beatae."
      subTitle2="Exercitationem, nihil!"
    />

    <div class="row">
      <div class="col-8  text-center">
        <div class="row">
          <div
            class="col-6 text-center"
            :key="data.id"
            v-for="data in compData"
          >
            <div class="p-2 row">
              <div
                class="col-3 d-flex align-items-center justify-content-center"
                v-html="data.icon"
              >
                <!-- change icons -->
              </div>
              <div class="col-9 text-left">
                <h6 class="pt-2 text-light">{{ data.text }}</h6>
                <p>{{ data.subText }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div
        class="
          p-2
          col-4 
          d-flex
          align-items-center
          justify-content-center
        "
      >
        <h1>IMAGE</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Features",
  data() {
    return {
      compData: [
        {
          id: 1,
          text: "Lorem ipsum",
          subText: "Duis aute irure dolor in dolore eu fugiat nulla pariatur.",
          icon: '<i class="fa-solid fa-gear fa-2xl"></i>',
        },
        {
          id: 2,
          text: "Sadipsum",
          subText: "Duis aute irure dolor in dolore eu fugiat nulla pariatur.",
          icon: '<i class="fa-solid fa-database fa-2xl"></i>',
        },
        {
          id: 3,
          text: "Sadipsum",
          subText: "Duis aute irure dolor in dolore eu fugiat nulla pariatur.",
          icon: '<i class="fa-solid fa-server fa-2xl"></i>',
        },
        {
          id: 4,
          text: "Sadipsum",
          subText: "Duis aute irure dolor in dolore eu fugiat nulla pariatur.",
          icon: '<i class="fa-solid fa-pen fa-2xl"></i>',
        },
      ],
    };
  },
};
</script>