<template>
  <div class="container-fluid text-center bg-light">
    <Title
      mainTitle="PRICING TABLE"
      subTitle1="Lorem ipsum dolor sit amet consectetur, adipisicing elit. In vitae inventore beatae."
      subTitle2="Exercitationem, nihil!"
    />

    <div class="row justify-content-center">
      <div
        class="mx-4 col-3 p-0 border"
        :key="data.id"
        v-for="data in compData"
      >
        <PriceComp
          :heading="data.heading"
          :price="data.price"
          :subText1="data.subText1"
          :subText2="data.subText2"
          :subText3="data.subText3"
          :subText4="data.subText4"
          :btnText="data.btnText"
        />
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "Pricing",
  data() {
    return {
      compData: [
        {
          id: 1,
          heading: "FREE",
          price: "$0",
          subText1: "Lorem ipsum dolor sit.",
          subText2: "Consectetur adipiscing elit",
          subText3: "Nunc vitae",
          subText4: "Vitae in eget met.",
          btnText: "Donecinia",
        },
        {
          id: 2,
          heading: "POPULAR",
          price: "$3.99",
          subText1: "Lorem ipsum dolor sit.",
          subText2: "Consectetur adipiscing elit",
          subText3: "Nunc vitae",
          subText4: "Vitae in eget met.",
          btnText: "Donecinia",
        },
        {
          id: 3,
          heading: "PREMIUM",
          price: "$5.99",
          subText1: "Lorem ipsum dolor sit.",
          subText2: "Consectetur adipiscing elit",
          subText3: "Nunc vitae",
          subText4: "Vitae in eget met.",
          btnText: "Donecinia",
        },
      ],
    };
  },
};
</script>

<style scoped>
.row {
  flex-wrap: nowrap;
}
</style>
