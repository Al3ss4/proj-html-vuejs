<template>
  <div class="container-fluid mt-5 subscribe-sec p-5">
    <div class="row">
      <div class="col-12 text-center mt-5">
        <h2>SubScribe <span class="orange">&</span> Receive A Free eBook</h2>
        <p>
          Aliquam erat volutpat. Ut quis ligula a magna blandit finibus.
          Suspendisse maximus lacus non nunc lacinia lobortis.
        </p>
      </div>
      <div class="col-12 d-flex justify-content-center">
        <form>
          <div class="form-group mt-5">
            <input
              type="email"
              class="form-control email-container"
              id="exampleInputEmail1"
              aria-describedby="emailHelp"
              placeholder="Insert your email...*"
            />
          </div>
        </form>
        <button type="button" class="btn btn-subscribe text-uppercase fw-bold">
          subscribe
        </button>
      </div>
      <p class="text-center mt-5">Cras porttitor pellentesque sem eu pretium.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "subscribeComponent",
};
</script>

<style lang="scss" scoped>
.subscribe-sec {
  background-image: url("@/assets/img/subscribe-sec-bg.png");
  background-position: center;
  background-size: cover;
}
.email-container {
  height: 50px;
  width: 600px;
}
h2 {
  line-height: 80px;
}
.orange {
  color: #fc7525;
}
.btn-subscribe {
  background-color: #fc7525;
  width: 15%;
  height: 60px;
  padding: 10px;
  color: white;
  border-radius: 0rem;
  margin-top: 43px;
  margin-left: 20px;
}
p{
    color: grey;
}
</style>