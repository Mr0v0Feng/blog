<template>
  <div class="CWeather">
    <div id="weather-float-he"></div>
  </div>
</template>

<script>
export default {
  mounted() {
    window.WIDGET = { FID: "0l18EudFEN" };
    (function(d) {
      var c = d.createElement("link");
      c.rel = "stylesheet";
      c.href =
        "https://apip.weatherdt.com/float/static/css/tqw_widget_float.css?v=0101";
      var s = d.createElement("script");
      s.src =
        "https://apip.weatherdt.com/float/static/js/tqw_widget_float.js?v=0101";
      var sn = d.getElementsByTagName("script")[0];
      sn.parentNode.insertBefore(c, sn);
      sn.parentNode.insertBefore(s, sn);
    })(document);
  }
};
</script>

<style lang="stylus">
#weather-float-he {
  top: 3.6rem !important;
  z-index: 1 !important;
  position: fixed !important;
}
</style>
