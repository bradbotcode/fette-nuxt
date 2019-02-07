<template>
    <div class="grid-container banner">
      <div class="grid-x">
        <div class="cell small-7">
          <h3 class="banner__headline">Precision is our Passion.</h3>
          <p>Call today to speak with a technical support representative or fill out our online form to kick start your next project. Thanks, and keep on rolling!</p>
        </div>

        <div class="cell small-5">
          <span class="banner__cta--call">
              <div>Call today:</div><br>888.888.8888
          </span>
          <div class="banner__cta--order">
            <router-link to="/contact">
              <button class="button">CONTACT FORM</button><br>
            </router-link>
          </div>
        </div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'BannerCtaSticky',
}
</script>
<style lang="scss" scoped>

  .banner {
    background-color: #101010;
    border-top: 1px solid gray;
    bottom: 0;
    left: 0;
    right: 0;
    padding: 18px 100px;
    position: fixed;
    width: 100%;
    z-index: 10;

    &__headline {
      color: white;
      font-family: "Roboto", sans-serif;
      font-weight: 900;
      font-size: 28px;
      margin-bottom: 0;
    }

    @media only screen and (max-width: 930px) {
      display: none;
    }
  }

  .banner__cta--call {
    color: white;
    font-family: "Roboto", sans-serif;
    font-weight: 900;
    font-size: 24px;
    float: right;
    line-height: 28px;
    margin-left: 18px;
    position: relative;
    top: 6px;

    div {
      font-family: "Oswald", sans-serif;
      font-size: 14px;
      margin-bottom: -32px;
    }
  }

  .banner__cta--order {
    border-right: 1px solid white;
    float: right;
    padding: 10px 18px 0 0;
  }

  .button {
    background-color: #ffae00;
    color: black;
    font-family: "Oswald", sans-serif;
  }

  p {
    color: white;
    font-family: "Oswald", sans-serif;
    margin-bottom: 0;
    width: 85%;
  }

  .small-5 {
    margin-top: 22px;
  }

  .small {
      font-size: 12px;
      margin: 0;
      padding: 0;
  }
</style>
