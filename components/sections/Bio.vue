<template>
  <div id="bio">
    <div class="container" style="z-index:4">
      <avatar />  
    </div>
    <div class="a-bg">
      <div class="container">
        <div class="a-container">
          <div class="a-summary">
            Ich bin freiberuflicher Webentwickler und ich begleite Unternehmen bei der Konzeption und Umsetzung ihrer digitalen Strategie.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.a-bg{
  background-color: var(--c-gray-1);
  position: relative;
  top: -40px;
}

.a-container{
  padding: 5rem 7rem;
}

.a-summary{
  padding: 1rem 0 1rem 3rem;
  border-left: 5px solid var(--c-purple-1);
  font-size: 2.2vw;
  color: var(--c-blue-1);
  font-weight: 300;
}

@media only screen and (max-width: 600px) {
  .a-summary {
    font-size: 1.8rem;
  }
  .a-container{
    padding: 5rem 0rem;
  }
}
</style>