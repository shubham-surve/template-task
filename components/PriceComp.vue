<template>
  <div class="text-center">
    <div class="bg-primary">
      <p class="m-0">{{ heading }}</p>
    </div>
    <!-- <table class="table">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">First</th>
          <th scope="col">Last</th>
          <th scope="col">Handle</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Mark</td>
          <td>Otto</td>
          <td>@mdo</td>
        </tr>
        <tr>
          <th scope="row">2</th>
          <td>Jacob</td>
          <td>Thornton</td>
          <td>@fat</td>
        </tr>
        <tr>
          <th scope="row">3</th>
          <td>Larry</td>
          <td>the Bird</td>
          <td>@twitter</td>
        </tr>
      </tbody>
    </table> -->

    <h1 class="pt-2">{{ price }}</h1>
    <div class="row"></div>
    {{ subText1 }}
    <hr />
    {{ subText2 }}
    <hr />
    {{ subText3 }}
    <hr />
    {{ subText4 }}
    <hr />
    <Button class="pb-3" :btnText="btnText" />
  </div>
</template>

<script>
export default {
  name: "PriceComp",
  props: {
    heading: String,
    price: String,
    subText1: String,
    subText2: String,
    subText3: String,
    subText4: String,
    btnText: String,
  },
};
</script>
