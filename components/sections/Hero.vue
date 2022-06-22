<template>
  <div class="a-bg">
    <div class="container">
      <div class="a-container">
        <div class="a-content">
          <div class="flex-v-s">
            <span class="a-title-1">Full Stack Development</span>
            <span class="a-title-2">E-Commerce</span>
          </div>
          <div class="flex">
            <jtl class="a-icon" />
            <shopify class="a-icon"  />
            <ebay class="a-icon"/>
          </div>
          <div>
            <a href="#bio" class="a-action">
              MEHR ERFAHREN
            </a>
          </div>
        </div>
        <div class="a-screenshots">
          <img src="~/assets/img/device-mockup.png"  class="a-img"/>
        </div>
      </div>
    </div>
    <div class="a-circle"/>
  </div>
</template>

<style scoped>

.a-container{
  position: relative;
  z-index: 3;
  height: 100vh;
}

.a-bg{
  position: relative;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background-color: var(--c-blue-1);
}

.a-action{
  all: unset;
  cursor: pointer;
  background-color: var(--c-purple-1);
  padding: 1.3em;
  color: white;
  border-radius: var(--border-radius);
  font-size: 1.6rem;
  font-weight: 600;
  transition: all 0.2s ease;
}

.a-action:hover{
  opacity: 0.8;
}

.a-content{
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  height: 100vh;
}

.a-title-1{
  font-size: 3rem;
  color: transparent;
  -webkit-text-stroke: 2px white;
  text-stroke: 2px solid white;
  font-weight: 900;
}

.a-title-2{
  font-size: 3rem;
  color: white;
  font-weight: 900;
}

.a-circle{
  position: absolute;
  right: 0;
  bottom: 0;
  width: 60vh;
  height: 60vh;
  transform: translateX(30%);
  background: linear-gradient(210.28deg, rgba(120, 55, 142, 0.51) 15.87%, rgba(38, 43, 50, 0) 75%);
  border-radius: 50%;
}

.a-screenshots{
  position: absolute;
  right: 0;
  bottom: 0;
  transform: translateY(40%);
}

.a-z3{
  z-index: 3;
}

.a-icon{
  height: 60px;
}

.a-img{
  height: 600px;
}

@media only screen and (max-width: 900px) {
  .a-img{
    height: 400px;
  }
}

@media only screen and (max-width: 600px) {
  .a-screenshots{
    position: absolute;
    left: 50%;
    bottom: 0;
    transform: translate(-50%, 40%);
  }
  .a-icon{
    height: 40px;
  }
  .a-img{
    height: 350px;
  }
  .a-content{
    height: calc(100vh - 250px);
  }
}

</style>