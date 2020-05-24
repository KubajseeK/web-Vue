<template>
  <div class="main-text">
      <h1 class="desc-title">
        {{description.title}}
      </h1>
      <p class="desc-subtitle">
        {{description.subtitle}}
      </p>
      <p class="desc-summary">
          {{description.summary}}
      </p>
      <p class="desc-summary2">
          {{description.summary2}}
      </p>
  </div>
</template>

<script>
export default {
    name: 'Description',
    props: ['description']
}
</script>

<style>
    .main-text {
        display: flex;
        flex-direction: column;
        text-align: center;
        justify-content: center;
        margin-top: 45px;
    }
    .desc-title {
        font-weight: 200;
        font-size: 2.2rem;
        color: hsl(240, 1%, 40%)
    }
    .desc-subtitle {
        font-weight: 600;
        font-size: 2.2rem;
        padding-bottom: 20px;
    }
    .desc-summary {
        color: hsl(229, 6%, 66%)
    }
    .desc-summary2 {
        color: hsl(229, 6%, 66%)
    }

    @media (max-width: 375px) {
        .main-text {
            margin-top: 70px;
        }

        .desc-title {
            font-size: 1.5rem;
        }
        .desc-subtitle {
            font-size: 1.5rem;
            padding-bottom: 10px;
        }
        .desc-summary {
            font-size: 1rem;
            padding: 0 50px
        }
        .desc-summary2 {
            font-size: 1rem;
            padding: 0 10px;
        }

    }

</style>