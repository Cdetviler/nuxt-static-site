<template>
  <Wrapper>
    <Card width="xl">
      <CardText 
        fontSize="4xl"
        :classes="['mb-3', 'tracking-widest', 'uppercase']"
      >
        About Charlie
      </CardText>
      <CardImage
        src="/charlieportrait.jpg"
        isRounded
        alt="Portrait of Charlie Detviler"
        alignment="center"
      />
      <CardText 
        fontSize="2xl"
        :classes="['mt-3']"
        color="accent"
      >
        I build functional and beautiful user interfaces.
      </CardText>
      <CardText 
        fontSize="md"
      >
        My work in advertising as well as traditional software development roles gives me a unique perspective on application design and development. I build React-based apps that make the user a priority.
      </CardText>
    </Card>
  </Wrapper>
</template>

<script>
import Wrapper from '~/components/Wrapper.vue'
import { Card, CardImage, CardText } from '~/components/Card'

export default {
  components: {
    Wrapper,
    Card,
    CardImage,
    CardText
  },
  layout: 'default'
}
</script>