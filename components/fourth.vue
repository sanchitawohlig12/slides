<template>
  <div class="fourth">
    <h1 class="header">How to create a web page.</h1>
    <div v-for="header in headers" :key="header.title" class="body">
      <h1 class="title">{{ header.title }}</h1>
      <p class="content">{{ header.content }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    headers: [
      {
        title: '1. Create an account.',
        content:
          'Sign up for a free Adobe Spark account online at spark.adobe.com or download the Adobe Spark Page app. Because your work automatically syncs across devices, you can get started on the web and iterate on-the-go or vice-versa.',
      },
      {
        title: '2. Pick a theme.',
        content:
          'Using Adobe Spark Page, choose a theme from the themes gallery to set fonts and styles that will completely transform your content’s look and feel. You can change it at any time by simply selecting another theme.',
      },
      {
        title: '3. Choose beautiful images to use.',
        content:
          'Add your images from your hard drive, Dropbox, or Lightroom account, or choose from thousands of royalty-free photos we provide.',
      },
      {
        title: '4. Add different elements to your web page.',
        content:
          'On your new page, choose from options to add text, buttons, images, or videos. Preview to see your work before it’s live.',
      },
      {
        title: '5. Share your page.',
        content:
          'When your page is complete, click share to get a new, unique URL. Your page is now ready to be shared across social media platforms, emailed, or added to newsletters and other publications. The Share tool can also generate a snippet of code that allows you to embed your new page into an existing website by pasting the code into your site files.',
      },
    ],
  }),
}
</script>

<style>
.header {
  text-align: center;
  margin-top: 08%;
  font-weight: 1200;
}
.body {
  margin-left: 5%;
  padding: 1%;
}
</style>