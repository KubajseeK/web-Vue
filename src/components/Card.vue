<template>
  <div class="card">
      <div :class="'card-inner ' + card.id">
        <div class="card-text-wrapper">
            <h3 class="card-title">{{card.title}}</h3>
            <span class="card-subtitle">{{card.subtitle}}</span>
        </div>
        <div class="card-image-wrapper">
            <img :src="card.imgsrc" class="image"/>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['card']
}
</script>

<style>
.card {
    width: 100%;
    padding: 25px;
    
}
    .card-inner {
    position: absolute;
    padding: 25px;
    box-shadow: 0px 10px 16px rgba(0, 0, 0, 0.15);
    background-color: white;
    border-width: 4px;
    border-radius: 10px;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    border-top-style: solid;
    width: 350px;
    height: 250px;
    

}
.card-inner.teambuilder {
    border-top-color: hsl(0, 78%, 62%);
    position: absolute;
    top: 300px;
    left: 550px;
    bottom: auto;
    right: auto;

}
.card-inner.karma {
    border-top-color: hsl(34, 97%, 64%);
    top: 580px;
    left: 550px;
    bottom: auto;
    right: auto;
    position: absolute;
}
.card-inner.calculator {
    border-top-color: hsl(212, 86%, 64%);
    position: absolute;
    top: 440px;
    left: 930px;
    bottom: auto;
    right: auto;
}
.card-inner.supervisor {
    border-top-color: hsl(180, 62%, 55%);
    top: 440px;
    left: 175px;
    bottom: auto;
    right: auto;
    position: absolute;
}

.card-image-wrapper .image {
    position: relative;
    margin: 0;
    top: 135px;
    left: 230px;
    bottom: 0px;
    right: 0px;
    width: 21%;
    
}

.card-text-wrapper {
    position: absolute;
    top: 30px;
    left: 20px;
    right: 0px;
    bottom: 0px;
    overflow: hidden;
    padding-left: 10px;
}

.card-text-wrapper h3 {
    margin-bottom: 15px;
    font-weight: 600;
    font-size: 1.2rem;
    
}
.card-text-wrapper span {
    color: hsl(229, 6%, 66%);
    font-size: 0.9rem;
}

@media (max-width: 375px) {
    
    .card-inner {
    padding: 25px;
    box-shadow: 0px 10px 16px rgba(0, 0, 0, 0.15);
    background-color: white;
    border-width: 4px;
    border-radius: 10px;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    border-top-style: solid;
    width: 300px;
    
}
.card-inner.teambuilder {
    border-top-color: hsl(0, 78%, 62%);
    position: absolute;
    top: 570px;
    left: 40px;
    bottom: auto;
    right: auto;
    

}
.card-inner.karma {
    border-top-color: hsl(34, 97%, 64%);
    top: 840px;
    left: 40px;
    bottom: auto;
    right: auto;
    position: absolute;
}
.card-inner.calculator {
    border-top-color: hsl(212, 86%, 64%);
    position: absolute;
    top: 1110px;
    left: 40px;
    bottom: auto;
    right: auto;
}
.card-inner.supervisor {
    border-top-color: hsl(180, 62%, 55%);
    top: 300px;
    left: 40px;
    bottom: auto;
    right: auto;
    position: absolute;
}

.card-image-wrapper .image {
    position: relative;
    margin: 0;
    top: 135px;
    left: 200px;
    bottom: 0px;
    right: 0px;
    width: 21%;
    
}

.card-text-wrapper {
    position: absolute;
    top: 30px;
    left: 20px;
    right: 0px;
    bottom: 0px;
    overflow: hidden;
    padding-left: 10px;
}

.card-text-wrapper h3 {
    margin-bottom: 15px;
    font-weight: 600;
    font-size: 1.2rem;
    
}
.card-text-wrapper span {
    color: hsl(229, 6%, 66%);
    font-size: 0.9rem;
}
}
</style>