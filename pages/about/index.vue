<template>
  <div>
    <PageSection>
      <Card width="xl">
        <CardText 
          fontSize="5xl"
          :classes="['mb-3', 'tracking-widest', 'uppercase', 'font-light']"
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
          I build functional and beautiful user interfaces
        </CardText>
        <CardText 
          fontSize="md"
        >
          My work in advertising as well as traditional software development roles gives me a unique perspective on application design and development. I build React-based apps that make the user a priority.
        </CardText>
      </Card>
    </PageSection>
    <PageSection inverted>
      <SectionHeader
        :classes="['tracking-widest', 'uppercase', 'mb-6']"
        fontSize="5xl"
        color="inverted"
      >
        Experience
      </SectionHeader>
      <ExperienceList />
    </PageSection>
  </div>
</template>

<script>
  import Wrapper from '~/components/Wrapper.vue';
  import { PageSection, SectionHeader } from '~/components/PageSection';
  import { Card, CardImage, CardText } from '~/components/Card';
  import ExperienceList from '~/components/ExperienceList.vue';

  export default {
    components: {
      Wrapper,
      Card,
      CardImage,
      CardText,
      PageSection,
      SectionHeader,
      ExperienceList
    },
    layout: 'default'
  }
</script>