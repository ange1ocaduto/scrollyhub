<template>
  <Head>
    <Title>Images & NFTs | {{ $config.projectMetadataTitle }}</Title>
    <Meta property="og:title" :content="'Images & NFTs | ' + $config.projectMetadataTitle" />
  </Head>

  <ChatFeed 
    class="mt-1" 
    :showQuotedPost="$config.showRepliesOnHomepage" 
    :orbisContext="$config.chatChannels.memesImages" 
  />
</template>

<script>
import ChatFeed from "../components/chat/ChatFeed.vue"

export default {
  name: "MemesImages",

  components: {
    ChatFeed
  }
}
</script>