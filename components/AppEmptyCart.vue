<template>
  <section v-if="!cart.length" class="emptycart">
    <svg
      height="200"
      width="200"
      fill="#000000"
      xmlns:x="http://ns.adobe.com/Extensibility/1.0/"
      xmlns:i="http://ns.adobe.com/AdobeIllustrator/10.0/"
      xmlns:graph="http://ns.adobe.com/Graphs/1.0/"
      xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink"
      version="1.1"
      x="0px"
      y="0px"
      viewBox="-949 951 100 100"
      style="enable-background: new -949 951 100 100"
      xml:space="preserve"
      aria-label="hungry"
      role="presentation"
    >
      <title id="hungry">Hungry Man Icon</title>
      <g>
        <g i:extraneous="self">
          <g>
            <path
              d="M-859.3,1003.3c-0.3,0.1-0.7,0.2-1.1,0.4c-2,0.9-13.7,6.5-13.7,6.5s-1.6-3.1-3.4-6.5c-1.8-3.4-3.9-7.2-4.9-8.5     c-1.4-1.8-3.2-3.3-5.2-4.3c-0.8-0.4-1.8-0.8-2.7-1.1c-2.5,1.8-5.6,2.8-8.9,2.8c-3.3,0-6.4-1-8.9-2.8c-1,0.3-1.8,0.7-2.7,1.1     c-2.1,1-3.8,2.5-5.2,4.3c-1.9,2.6-8.4,15.1-8.4,15.1s-3-1.5-6.2-3c-3.2-1.5-6.6-3.2-7.4-3.5c-0.3-0.1-0.5-0.2-0.8-0.2l-3,7.7     c0.4,0.3,0.8,0.6,1.3,0.8c3,1.4,17.1,8.6,18.4,8.9c1.3,0.3,2.9-0.7,3.6-2.1l6.4-12.7l-2.5,26.4c-0.1,1.6,0.9,3,2.5,3.2     c4.2,0.6,8.5,0.9,12.9,0.9c4.3,0,8.5-0.3,12.5-0.9c1.6-0.2,2.7-1.6,2.5-3.2l-2.5-26.4l6.5,12.7c0.7,1.4,2,2.5,3.6,2.1     c1.6-0.4,14.7-7.1,18.4-8.9c0.6-0.3,1.2-0.6,1.6-1c0,0,0-0.1,0-0.1L-859.3,1003.3z"
            ></path>
            <circle cx="-899.2" cy="977" r="11.7"></circle>
            <path
              d="M-851.7,1008.8l-5.2-9.3l0.3-0.2c1-0.5,1.4-1.8,0.7-2.7l-3.9-5.8c-0.5-0.7-1.4-1-2.2-0.6c-0.3,0.1-0.4,0.5-0.3,0.7l2.5,6     l5.2,13.3c0.3,0.8,1.3,1.2,2.1,0.8l0.1-0.1C-851.6,1010.6-851.3,1009.6-851.7,1008.8z"
            ></path>
            <path
              d="M-937.7,998.7c0.6-0.2,1.1-0.7,1.4-1.3l0.3-0.6h0l0,0l2.1-4.8c0.1-0.2,0-0.4-0.1-0.6c-0.2-0.2-0.6-0.1-0.7,0.2     c0,0-1.7,3.5-2.2,4.4c-0.1,0.1-0.2,0.2-0.4,0.1l0,0c-0.1-0.1-0.2-0.2-0.1-0.4c0.5-1,2-4.5,2-4.5c0.1-0.3,0-0.6-0.3-0.6     c-0.2-0.1-0.4,0.1-0.5,0.3l-2.2,4.4c-0.1,0.1-0.2,0.2-0.4,0.1c0,0,0,0,0,0c-0.1-0.1-0.2-0.2-0.1-0.4c0.5-1,2-4.5,2-4.5     c0.1-0.3,0-0.6-0.3-0.6c-0.2-0.1-0.4,0.1-0.5,0.3l-2.4,4.7l0,0h0l-0.3,0.6c-0.3,0.6-0.4,1.3-0.2,1.9l0.4,1.2l-6,10.7     c-0.4,0.8-0.1,1.8,0.7,2.2l0.1,0.1c0.8,0.4,1.8,0,2.1-0.8l4.5-11.4L-937.7,998.7z"
            ></path>
          </g>
        </g>
      </g>
    </svg>
    <h3>Your cart is empty!</h3>
    <nuxt-link exact to="/">
        <button class="primary">Fill it up!</button>
    </nuxt-link>
  </section>
</template>

<script>
import { mapState } from "vuex";

export default {
      computed: {
    ...mapState(["cart"]),
  },
};
</script>

<style lang="scss" scoped>
</style>