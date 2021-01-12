<template>
  <b-row no-gutters class="h-100 coming-soon justify-content-center">
      <div class="my-auto">
        <img :src="logo" alt="ForEach Group" class="img-fluid mx-auto mylogo">
        <div class="title">{{ title }}</div>
        <div class="disclaimer font-weight-light">
          <vue-typed-js
            class="d-block"
            :loop="true"
            :strings="disclaimer"
          >
          <span class="typing"></span>
          </vue-typed-js>
        </div>
      </div>
  </b-row>
</template>

<script>
export default {
  name: "ComingSoon",
  data(){
    return {
      logo: require('@/assets/logo.png'),
      title: 'ForEachGroup.com',
      disclaimer:[
        'Oooh, hello curious soul ;)', 
        'You are obviously interested in ???',
        'Software or Hardware :O',
        'Maybe you are an engineer ?',
        'Or you need someone to help you...',
        'With design, performance, architecture ',
        'Or you need to brainstorm idea a bit ?',
        'This basic animation is here to...',
        'Tell you that we would love to hear ',
        "What's on your mind !!!",
        'Please be kind and send us an email to:',
        'soul [at] foreachgroup.com',
        'Have a great day! And be AWESOME :)'
      ],
    }
  }
}
</script>

<style lang="scss" scoped>
.coming-soon{

  background: linear-gradient(90deg, rgba(20,19,43,1) 0%, rgba(101,12,113,1) 100%);

  .title{
    font-size: 1rem;
    text-align: right;
    padding-right: 1.5rem;
    color: white;
  }

  .disclaimer{
    font-size: 1.6rem;
    color: white;
    padding-left: 1rem;
  }

  .mylogo {
    padding: 0.6rem;
  }
}
</style>
