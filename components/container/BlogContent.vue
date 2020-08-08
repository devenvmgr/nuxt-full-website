<template>
  <section class="my-12">
    <div class="text-center">
      <h2 class="text-6xl">I'm a blog title</h2>
      <p>I'm the date and author</p>
    </div>

    <article>
      <p>Vitae congue eu consequat ac felis donec. Elit pellentesque habitant morbi tristique senectus et netus et malesuada. Amet venenatis urna cursus eget nunc scelerisque viverra mauris. Mi ipsum faucibus vitae aliquet nec. Egestas purus viverra accumsan in nisl nisi. Arcu non odio euismod lacinia at. Nunc lobortis mattis aliquam faucibus purus. Diam quis enim lobortis scelerisque fermentum dui faucibus in ornare. Metus aliquam eleifend mi in. Ultrices mi tempus imperdiet nulla malesuada pellentesque.</p>
      <p>At tempor commodo ullamcorper a. Mauris commodo quis imperdiet massa tincidunt. Odio ut enim blandit volutpat maecenas volutpat blandit aliquam. Diam quam nulla porttitor massa id neque aliquam vestibulum. Luctus accumsan tortor posuere ac ut consequat semper viverra nam. Mauris ultrices eros in cursus. Erat pellentesque adipiscing commodo elit at imperdiet dui accumsan. Scelerisque felis imperdiet proin fermentum leo vel orci porta non. Ac tortor dignissim convallis aenean et tortor at risus.</p>
      <p>Bibendum enim facilisis gravida neque convallis a. Euismod in pellentesque massa placerat duis ultricies lacus sed turpis. Massa tincidunt dui ut ornare lectus sit amet est placerat. Ultrices tincidunt arcu non sodales neque sodales ut etiam. Nunc mi ipsum faucibus vitae aliquet nec ullamcorper. Mauris sit amet massa vitae tortor condimentum lacinia. Ullamcorper malesuada proin libero nunc consequat interdum varius. Ut consequat semper viverra nam. Auctor eu augue ut lectus arcu bibendum at varius. At varius vel pharetra vel.</p>

      <buttons>123</buttons>
    </article>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
p {
  padding-bottom: 2rem;
}

article {
  column-width: 16rem;
  line-height: 1.5;
  /* width: 45rem; */
  width: 90%;
  column-gap: 2rem;
  margin: 2rem auto;
  text-align: justify;
  /* widows: 2; */
  /* position: relative;
  column-fill: balance;
  position: relative; */
  /* background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/tie.svg);
  background-repeat: no-repeat;
  background-position: center; */
}
article p:first-of-type {
  margin-top: 0;
}
</style>
