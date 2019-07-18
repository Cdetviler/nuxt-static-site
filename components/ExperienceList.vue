<template>
  <div>
    <Card width="full" class="mb-4">
      <CardText
        fontSize="2xl"
        :classes="['mb-2']"
        color="inverted"
        alignment="left"
      >
        Front-End Developer - Nevelex
      </CardText>
      <CardList
        :listItems="[
          'Engages in Agile software development methodologies such as Scrum and Kanban.',
          'Develops and improves intuitive applications in React and Redux.',
          'Constructs user interfaces that communicate with a Django backend using the Django REST Framework.',
          'Conducts meetings, embraces leadership roles, and takes point on front-end development tasks.',
          'Educates colleagues on the fundamentals of React through company-wide tech talk lectures.'
        ]"
      />
    </Card>
    <Card width="full" class="mb-4">
      <CardText
        fontSize="2xl"
        :classes="['mb-2']"
        color="inverted"
        alignment="left"
      >
        Web Developer Consultant - Digisage
      </CardText>
      <CardList
        :listItems="[
          'Revamped and mantained large WordPress website, Castle Realty.',
          'Collaborated with a team to create robust, modern web products and WordPress templates.'
        ]"
      />
    </Card>
    <Card width="full" class="mb-4">
      <CardText
        fontSize="2xl"
        :classes="['mb-2']"
        color="inverted"
        alignment="left"
      >
        Web Developer - Vendi
      </CardText>
      <CardList
        :listItems="[
          'Utilized content management systems like WordPress and Drupal to shape client-friendly web solutions',
          'Created an automated script to reduce the workload of colleagues and maximize profits.',
          'Bolstered non-profits and local organizations as lead developer on several projects through Vendi Share.'
        ]"
      />
    </Card>
    <Card width="full" class="mb-4">
      <CardText
        fontSize="2xl"
        :classes="['mb-2']"
        color="inverted"
        alignment="left"
      >
        Front-End Developer - APRS World
      </CardText>
      <CardList
        :listItems="[
          'Operated as the sole Web Developer to improve and maintain the existing company website.',
          'Used web frameworks and libraries to create software featuring live camera feeds and sensor data.',
          'Developed and tested RESTful web applications with emphasis on User Experience.'
        ]"
      />
    </Card>
  </div>
</template>

<script>
  import { Card, CardText, CardList } from '~/components/Card';

  export default {
    components: {
      Card,
      CardText,
      CardList
    },
  }
</script>

<style scoped>

</style>