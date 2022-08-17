<template>
  <div div class="container-fluid text-center bg-light">
    <div class="row mx-5">
      <div class="col text-left m-5">
        <h3 class="pb-3">
          {{ compData.title }}
        </h3>
        <small>
          <p>{{ compData.address }}</p>
          <p>
            Phone:
            <span class="text-muted"
              >{{ "&#40;" }}{{ compData.phoneNum }}{{ "&#41;" }}</span
            >
          </p>
          <p>
            E-mail:
            <span class="text-muted"
              >{{ "&#40;" }}{{ compData.email }}{{ "&#41;" }}</span
            >
          </p>
          <div>logo</div>
        </small>
      </div>
      <div class="col m-5">
        <form action="">
          <div class="form-group">
            <input
              type="text"
              class="form-control mb-2 bg-light"
              placeholder="Your Name"
            />
            <input
              type="email"
              class="form-control my-2 bg-light"
              placeholder="Your email"
            />
            <textarea
              class="form-control my-2 bg-light"
              rows="5"
              placeholder="Your Text"
            ></textarea>
          </div>
        </form>
        <Button btnText="SEND MESSAGE" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  Name: "Contact",
  data() {
    return {
      compData: {
        title: "Contact With Us",
        address: "Building,road,state.",
        phoneNum: "+91 123456789",
        email: "example@mate.com",
      },
    };
  },
};
</script>
