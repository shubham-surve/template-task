<template>
  <div div class="container-fluid text-center bg-secondary">
    <Title
      mainTitle="RECENT BLOG"
      subTitle1="Lorem ipsum dolor sit amet consectetur, adipisicing elit. In vitae inventore beatae."
      subTitle2="Exercitationem, nihil!"
    />

    <div class="border-danger row p-0 mx-5">
      <div class="col text-left p-0 m-4" :key="data.id" v-for="data in compData">
        <img class="img-fluid w-100" :src="data.img" alt="img">
        <h5 class="pt-2">{{data.sub}}</h5>
        <p>{{data.para}}</p>
        
      </div>
    </div>
  </div>  
</template>

<script>
import img2 from '~/assets/images/img2.jpeg'

export default {
  name: 'Blog',
  data() {
    return {
      compData: [
        {
          id:1,
          img:img2,
          sub:'Lorem',
          para:'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam',
        },
        {
          id:2,
          img:img2,
          sub:'Lorem',
          para:'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam'
        },
        {
          id:2,
          img:img2,
          sub:'Lorem',
          para:'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam'
        }
      ],
    };
  },
};
</script>