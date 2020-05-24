<template>
  <div id="app">
    <Description
    v-for="desc in description"
    :key="desc"
    :description="desc"
    />
    <div class="cards">
      <Card
      v-for="card in cards"
      :key="card"
      :card="card"
      />
    </div>
  </div>
</template>

<script>
import Card from './components/Card'
import Description from './components/Description'


export default {
  name: 'App',
  components: {
    Card,
    Description
  },
  data() {
    return {
      cards: [
        {
          title: 'Team Builder',
          subtitle: 'Scans out talent network to create the optimal team for your project',
          id: 'teambuilder',
          imgsrc: require('./assets/icon-team-builder.svg')
        },
        {
          title: 'Supervisor',
          subtitle: 'Monitors activity to identify project roadblocks',
          id: 'supervisor',
          imgsrc: require('./assets/icon-supervisor.svg')
        },
        {
          title: 'Karma',
          subtitle: 'Regularly evaluates our talent to ensure quality',
          id: 'karma',
          imgsrc: require('./assets/icon-karma.svg')
        },
        {
          title: 'Calculator',
          subtitle: 'Uses data from past projects to provide better delivery estimates',
          id: 'calculator',
          imgsrc: require('./assets/icon-calculator.svg')
        }
      ],
      description: [
        {
        title: 'Reliable, efficient delivery',
        subtitle: 'Powered by Technology',
        summary: 'Our Artificial Intelligence powered tools use millions of project data',
        summary2: 'points to ensure that your project is successful'
        }
      ]
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
  font-size: 15px;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background-color: hsl(0, 0%, 98%);
  
}

.cards {
  display: flex;
  min-width: 20px;
  min-height: 20px;
  padding: 25px;
  margin: 0 auto;
}
</style>
