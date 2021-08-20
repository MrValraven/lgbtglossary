<template>
  <Navbar />
  <section class="hero">
    <div class="heroText">
      <h1>A begineer's guide to</h1>
      <h2>
        <span>L</span>
        <span>G</span>
        <span>B</span>
        <span>T</span>
        <span>Q</span>
        <span>I</span>
        <span>A</span>
        <span>+</span>
      </h2>
      <p>Show your support by learning more about the community</p>
      <button>Learn more</button>
    </div>
    <div class="heroImage">
      <img src="@/assets/pride.svg" alt="">
    </div>
  </section>
  <section class="terms">
    <img src="@/assets/lgbt.png" alt="">
    <ul>
      <li>Lesbian</li>
      <li>Gay</li>
      <li>Bisexual</li>
      <li>Transgender</li>
      <li>Queer</li>
      <li>Asexual Aromantic</li>
      <li>Intersex</li>
      <li>+ Broader spectrum of identities</li>
    </ul>
  </section>
  <section>
    <p>The term LGBTQ+ represents the community of people whose sexual or gender identity does not conform to current societal norms.</p>
    <p>The acronym refers to some of these specific identities, yet it represents the community as a whole.</p>
  </section>
  <Footer />
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Navbar,
    Footer,
  }
}
</script>

<style scoped lang="scss">

$easing: cubic-bezier(0.075, 0.82, 0.165, 1);
$animationTime: 1s;

@keyframes scaleUp {
  0% {
    transform: scale(0);
    opacity: 1;
  }

  100% {
    transform: scale(1);
    opacity: 1;
  }
}

section {
  padding: 50px 100px;
}

.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 0;
  height: 95vh;

  .heroText {
    width: 50%;
    margin-top: -125px;


    h1 {
      font-size: 20px;
      margin: 0;
    }

    h2 {
      font-size: 120px;
      margin: -40px 0 0 0;

      span {
        display: inline-block;
        opacity: 0;

        &:nth-child(1) {
          color: #FF0000;
          animation: scaleUp $animationTime $easing 0.5s both;
        }
        &:nth-child(2) {
          color: #FF7F00;
          animation: scaleUp $animationTime $easing 0.6s both;
        }
        &:nth-child(3) {
          color: #FFFF00;
          animation: scaleUp $animationTime $easing 0.7s both;
        }
        &:nth-child(4) {
          color: #00FF00;
          animation: scaleUp $animationTime $easing 0.8s both;
        }
        &:nth-child(5) {
          color: #0000FF;
          animation: scaleUp $animationTime $easing 0.9s both;
        }
        &:nth-child(6) {
          color: #2E2B5F;
          animation: scaleUp $animationTime $easing 1.0s both;
        }
        &:nth-child(7) {
          color: #8B00FF;
          animation: scaleUp $animationTime $easing 1.1s both;
        }
        &:nth-child(8) {
          color: #FF0000;
          animation: scaleUp $animationTime $easing 1.2s both;
        }

      }
    }

    p {
      margin-top: 0;
    }

    button {
      padding: 1rem 1.5rem;
      border-radius: 25px;
      cursor: pointer;
      outline: none;
    }
  }

  .heroImage {
    width: 40%;
    z-index: -2;

  }
}

.terms {
  padding: 0;

  img {
    width: 600px;
  }

  ul {
    list-style: none;

    li {
      font-weight: 600;
      font-size: 50px;
      width: 350px;
      text-align: right;
      text-transform: uppercase;
      border: 2px solid red;

      &:nth-child(1) {
        margin-left: -50px;
      }
    }
  }
}

</style>
