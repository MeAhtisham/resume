<template>
  <section id="map">
    <b-container fluid>
      <b-row>
        <b-col p-0>
          <div class="mapouter"
            ><div class="gmap_canvas"
              ><iframe
                class="gmap_iframe"
                width="100%"
                frameborder="0"
                scrolling="no"
                marginheight="0"
                marginwidth="0"
                src="https://maps.google.com/maps?width=600&amp;height=400&amp;hl=en&amp;q=gilgit pakistan&amp;t=p&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"
              ></iframe
              ><a
                href="https://www.fridaynightfunkin.net/friday-night-funkin-mods-fnf-play-online/"
                >Friday Night Funkin Mods</a
              ></div
            ></div
          >
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#map {
  overflow: hidden;
}
.container-fluid {
  padding: 0px !important;
  /* overflow: hidden !important; */
}
.mapouter {
  position: relative;
  text-align: right;
  width: 100%;
  height: 400px;
}
.gmap_canvas {
  overflow: hidden;
  background: none !important;
  width: 100%;
  height: 400px;
}
.gmap_iframe {
  height: 400px !important;
}
</style>
