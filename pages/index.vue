<template>
  <div>
    <Header />
    <HeroImage />
    <CenterCtaFull />

    <ModalButton />
    <CenterCta size="narrow" button="false" />
    <ImageSlider />

    <div class="flex">
      <ImageColumns />
      <ImageColumns />
      <ImageColumns />
      <ImageColumns />
    </div>

    <Timeline />
    <ProductHero />

    <div class="flex justify-around">
      <ProductDisplayAll total="4" />
      <ProductDisplayAll total="4" />
      <ModalButtonMega />
    </div>

    <div class="flex">
      <Testimonials />
      <Testimonials />
      <Testimonials />
      <Testimonials />
    </div>

    <BlogContent />
    <SocialButtons />
    <FormContact />

    <!-- <div class="container">
      <div>
        <logo />
        <h1 class="title">nuxt-full-BUTT</h1>
        <h2 class="subtitle">My peachy Nuxt.js project</h2>
        <div class="links">
          <a href="https://nuxtjs.org/" target="_blank" class="button--green">Documentation</a>
          <a href="https://github.com/nuxt/nuxt.js" target="_blank" class="button--grey">GitHub</a>
        </div>
      </div>
    </div>-->

    <Footer />
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Header from '~/components/container/Header.vue'
import HeroImage from '~/components/container/HeroImage.vue'
import CenterCta from '~/components/container/CenterCta.vue'
import CenterCtaFull from '~/components/container/CenterCtaFull.vue'
import ImageSlider from '~/components/container/ImageSlider.vue'
import ImageColumns from '~/components/container/ImageColumns.vue'
import Timeline from '~/components/container/Timeline.vue'
import ProductHero from '~/components/container/ProductHero.vue'
import ProductDisplayAll from '~/components/container/ProductDisplayAll.vue'
import Testimonials from '~/components/container/Testimonials.vue'
import BlogContent from '~/components/container/BlogContent.vue'
import SocialButtons from '~/components/container/SocialButtons.vue'
import FormContact from '~/components/container/FormContact.vue'
import Footer from '~/components/container/Footer.vue'

import ModalButton from '~/components/container/ModalButton.vue'
import ModalButtonFull from '~/components/container/ModalButtonFull.vue'

export default {
  components: {
    Header,
    HeroImage,
    ModalButton,
    ModalButtonFull,
    CenterCta,
    CenterCtaFull,
    ImageSlider,
    ImageColumns,
    Timeline,
    ProductHero,
    ProductDisplayAll,
    Testimonials,
    BlogContent,
    SocialButtons,
    FormContact,
    Logo,
    Footer
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
