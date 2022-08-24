<template>
  <div class="gallery-card1-gallery-card" v-bind:class="rootClassName">
    <img :alt="image_alt" :src="image_src" class="gallery-card1-image" />
    <h2 class="gallery-card1-text">{{ title }}</h2>
  </div>
</template>

<script>
export default {
  name: 'GalleryCard1',
  props: {
    title: {
      type: String,
      default: 'Project Title',
    },
    image_alt: {
      type: String,
      default: 'image',
    },
    rootClassName: String,
    image_src: {
      type: String,
      default:
        'https://images.unsplash.com/photo-1418065460487-3e41a6c84dc5?ixid=Mnw5MTMyMXwwfDF8c2VhcmNofDEyfHxmb3Jlc3R8ZW58MHx8fHwxNjI2MjUxMjg4&ixlib=rb-1.2.1&w=1500',
    },
  },
}
</script>

<style scoped>
.gallery-card1-gallery-card {
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.gallery-card1-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.gallery-card1-text {
  align-self: center;
  margin-top: var(--dl-space-space-halfunit);
  font-weight: 600;
  margin-bottom: var(--dl-space-space-halfunit);
}



@media(max-width: 991px) {
  .gallery-card1-gallery-card {
    width: auto;
  }
  .gallery-card1-image {
    width: 300px;
    height: 300px;
  }
  .gallery-card1-root-class-name {
    width: auto;
  }
  .gallery-card1-root-class-name1 {
    width: auto;
  }
  .gallery-card1-root-class-name2 {
    width: auto;
  }
}
@media(max-width: 767px) {
  .gallery-card1-gallery-card {
    width: auto;
    flex-direction: column;
  }
  .gallery-card1-image {
    width: 250px;
    height: 250px;
  }
}
@media(max-width: 479px) {
  .gallery-card1-gallery-card {
    width: auto;
  }
  .gallery-card1-image {
    width: 150px;
    height: 150px;
  }
}
</style>
