<template>
  <main>
    <section>
      <content-carousel
        :type="'rss'"
        :source="'/hero.rss'"
        :slick-options="heroOptions"
        :carousel-height="heroHeight"
        :fit-to-container="true"
        :text-align="alignText"
      />
    </section>
    <section class="content">
      <content-carousel
        :type="'rss'"
        :source="'/content.rss'"
        :slick-options="contentOptions"
        :carousel-height="contentHeight"
      />
    </section>
    <section class="content">
      <content-carousel
        :type="'rss'"
        :source="'/empty.rss'"
        :slick-options="contentOptions"
        :carousel-height="contentHeight"
      />
    </section>
    <section class="content">
      <content-carousel
        :type="'portlet'"
        :source="'/portletRegistry.json'"
        :slick-options="portletOptions"
        :carousel-height="portletHeight"
      />
    </section>
    <section class="content">
      <content-carousel
        :type="'passthrough'"
        :slick-options="contentOptions"
        :carousel-height="portletHeight"
      >
        <div class="slick-item">
          arbitrary
        </div>
        <div class="slick-item">
          content
        </div>
        <div class="slick-item">
          displayed
        </div>
        <div class="slick-item">
          as
        </div>
        <div class="slick-item">
          slides
        </div>
      </content-carousel>
    </section>
  </main>
</template>
<script lang="ts" src="./App.ts">
</script>
<style lang="scss" src="./App.scss">
</style>
