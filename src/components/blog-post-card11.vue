<template>
  <div class="blog-post-card11-blog-post-card" v-bind:class="rootClassName">
    <img :alt="image_alt" :src="image_src" class="blog-post-card11-image" />
    <div class="blog-post-card11-container">
      <span class="blog-post-card11-text">{{ title }}</span>
      <span class="blog-post-card11-text1">{{ zipname2 }}</span>
      <span class="blog-post-card11-text2">{{ pkgname2 }}</span>
      <span class="blog-post-card11-text3">{{ md53 }}</span>
      <span class="blog-post-card11-text4">{{ md521 }}</span>
      <span class="blog-post-card11-text5">{{ zipname }}</span>
      <span class="blog-post-card11-text6">{{ time2 }}</span>
      <span class="blog-post-card11-text7">{{ au }}</span>
      <span class="blog-post-card11-text8">{{ au2 }}</span>
      <button class="blog-post-card11-button button">{{ button }}</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BlogPostCard11',
  props: {
    md53: {
      type: String,
      default: 'md5',
    },
    rootClassName: String,
    zipname: {
      type: String,
      default: '构建时间',
    },
    pkgname2: {
      type: String,
      default: 'miui_CMIPRE_22.8.19_dc9f802608_12.0.zip',
    },
    au: {
      type: String,
      default: '维护者',
    },
    button: {
      type: String,
      default: '下载',
    },
    zipname2: {
      type: String,
      default: '包名',
    },
    au2: {
      type: String,
      default: '维护者',
    },
    title: {
      type: String,
      default: 'device',
    },
    md521: {
      type: String,
      default: 'dc9f8026089f36a8af4d851ea3772403',
    },
    image_alt: {
      type: String,
      default: 'image',
    },
    time2: {
      type: String,
      default: 'time',
    },
    image_src: {
      type: String,
      default:
        'https://images.unsplash.com/photo-1547841243-eacb14453cd9?ixid=Mnw5MTMyMXwwfDF8c2VhcmNofDIyfHxjaXR5fGVufDB8fHx8MTYyNjE4NjYxMg&ixlib=rb-1.2.1&h=400',
    },
  },
}
</script>

<style scoped>
.blog-post-card11-blog-post-card {
  width: 100%;
  display: flex;
  overflow: hidden;
  max-width: var(--dl-size-size-maxwidth);
  box-shadow: 5px 5px 10px 0px rgba(18, 18, 18, 0.1);
  transition: 0.3s;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.blog-post-card11-blog-post-card:hover {
  transform: scale(1.02);
}
.blog-post-card11-image {
  width: 300px;
  height: 400px;
  object-fit: cover;
}
.blog-post-card11-container {
  display: flex;
  padding: var(--dl-space-space-twounits);
  align-self: flex-start;
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.blog-post-card11-text {
  font-size: 28px;
  font-style: normal;
  font-weight: 700;
  margin-bottom: var(--dl-space-space-twounits);
}
.blog-post-card11-text1 {
  color: var(--dl-color-gray-500);
  font-size: 20px;
  font-style: normal;
  font-weight: 600;
  margin-bottom: 0px;
}
.blog-post-card11-text2 {
  color: var(--dl-color-gray-500);
  font-style: normal;
  font-weight: 400;
  margin-bottom: var(--dl-space-space-halfunit);
}
.blog-post-card11-text3 {
  color: var(--dl-color-gray-500);
  font-size: 20px;
  font-style: normal;
  font-weight: 600;
  margin-bottom: 0px;
}
.blog-post-card11-text4 {
  color: var(--dl-color-gray-500);
  font-weight: 400;
  margin-bottom: var(--dl-space-space-halfunit);
}
.blog-post-card11-text5 {
  color: var(--dl-color-gray-500);
  font-size: 20px;
  font-style: normal;
  font-weight: 600;
  margin-bottom: 0px;
}
.blog-post-card11-text6 {
  color: var(--dl-color-gray-500);
  font-weight: 400;
  margin-bottom: var(--dl-space-space-halfunit);
}
.blog-post-card11-text7 {
  color: var(--dl-color-gray-500);
  font-size: 20px;
  font-style: normal;
  font-weight: 600;
  margin-bottom: 0px;
}
.blog-post-card11-text8 {
  color: var(--dl-color-gray-500);
  font-weight: 400;
  margin-bottom: var(--dl-space-space-unit);
}
.blog-post-card11-button {
  color: var(--dl-color-gray-white);
  border-width: 0px;
  background-color: #E76510;
}





@media(max-width: 1600px) {
  .blog-post-card11-image {
    width: 300px;
    height: 400px;
  }
  .blog-post-card11-container {
    align-self: flex-start;
  }
  .blog-post-card11-text {
    font-size: 28px;
    font-style: normal;
    font-weight: 700;
  }
  .blog-post-card11-text1 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text2 {
    margin-bottom: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text3 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text4 {
    margin-bottom: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text5 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text6 {
    margin-bottom: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text7 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text8 {
    margin-bottom: var(--dl-space-space-unit);
  }
  .blog-post-card11-button {
    color: var(--dl-color-gray-white);
    border-width: 0px;
    background-color: #E76510;
  }
}
@media(max-width: 1200px) {
  .blog-post-card11-image {
    width: 300px;
    height: 400px;
  }
  .blog-post-card11-container {
    padding: var(--dl-space-space-unit);
    align-self: flex-start;
  }
  .blog-post-card11-text {
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
  }
  .blog-post-card11-text1 {
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text2 {
    font-size: 14px;
    margin-bottom: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text3 {
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text4 {
    font-size: 14px;
    margin-bottom: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text5 {
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text6 {
    font-size: 14px;
    margin-bottom: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text7 {
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text8 {
    font-size: 14px;
    margin-bottom: var(--dl-space-space-unit);
  }
  .blog-post-card11-button {
    color: var(--dl-color-gray-white);
    border-width: 0px;
    background-color: #E76510;
  }
  .blog-post-card11-root-class-name1 {
    width: auto;
  }
  .blog-post-card11-root-class-name2 {
    width: auto;
  }
  .blog-post-card11-root-class-name3 {
    width: auto;
  }
}
@media(max-width: 991px) {
  .blog-post-card11-blog-post-card {
    width: 697px;
    align-items: center;
    flex-direction: row;
    justify-content: center;
  }
  .blog-post-card11-image {
    width: 300px;
    height: 400px;
    align-self: flex-start;
  }
  .blog-post-card11-container {
    align-self: center;
  }
  .blog-post-card11-text {
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
  }
  .blog-post-card11-text1 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text3 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text5 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text7 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-button {
    color: var(--dl-color-gray-white);
    width: 72px;
    height: 36px;
    font-size: 16px;
    align-self: flex-start;
    text-align: center;
    border-width: 0px;
    background-color: #E76510;
  }
}
@media(max-width: 767px) {
  .blog-post-card11-text {
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
  }
  .blog-post-card11-text1 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text3 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text5 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-text7 {
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 0px;
  }
  .blog-post-card11-button {
    color: var(--dl-color-gray-white);
    width: 72px;
    height: 36px;
    align-self: flex-start;
    text-align: center;
    line-height: auto;
    border-width: 0px;
    background-color: #e76510;
  }
}
@media(max-width: 479px) {
  .blog-post-card11-blog-post-card {
    width: auto;
  }
  .blog-post-card11-image {
    width: 166px;
    height: 222px;
    align-self: center;
    margin-top: 5px;
    margin-left: 5px;
    margin-right: 5px;
    margin-bottom: 5px;
  }
  .blog-post-card11-container {
    width: 260px;
    padding-left: var(--dl-space-space-halfunit);
    padding-right: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text {
    font-size: 20px;
    font-style: normal;
    font-weight: 700;
    margin-bottom: var(--dl-space-space-halfunit);
  }
  .blog-post-card11-text1 {
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 2px;
  }
  .blog-post-card11-text2 {
    font-size: 10px;
  }
  .blog-post-card11-text3 {
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 2px;
  }
  .blog-post-card11-text4 {
    font-size: 10px;
  }
  .blog-post-card11-text5 {
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 2px;
  }
  .blog-post-card11-text6 {
    font-size: 10px;
  }
  .blog-post-card11-text7 {
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 2px;
  }
  .blog-post-card11-text8 {
    font-size: 10px;
  }
  .blog-post-card11-button {
    color: #ffffff;
    width: 57px;
    height: var(--dl-size-size-small);
    margin: 0px;
    font-size: 10px;
    align-self: flex-start;
    align-items: center;
    line-height: 1.9;
    padding-top: 0px;
    border-style: solid;
    border-width: 0px;
    padding-left: 0px;
    padding-right: 0px;
    padding-bottom: 0px;
    justify-content: center;
    background-color: #e76510;
  }
  .blog-post-card11-root-class-name1 {
    width: 370px;
  }
  .blog-post-card11-root-class-name2 {
    width: 370px;
  }
  .blog-post-card11-root-class-name3 {
    width: 370px;
  }
}
</style>
