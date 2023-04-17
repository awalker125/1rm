<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Instructions</template>
    Type in the numbers of reps and kgs you lifted and we'll calculator and estimate of your 1 rep max.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Formula</template>

    The formula used is called the Epley formula <a href="https://en.wikipedia.org/wiki/One-repetition_maximum">1</a> <a
      href="https://www.omnicalculator.com/sports/one-rep-max">2</a>. It is used to estimate a person’s one-repetition
    maximum (1RM) based on their performance in a weightlifting exercise <a
      href="https://en.wikipedia.org/wiki/One-repetition_maximum">1</a>. The formula was developed by Dr. Epley in 1985 3.

    However, there are other formulas that can be used to estimate a person’s 1RM, such as the Brzycki formula and the
    Lander formula <a href="https://en.wikipedia.org/wiki/One-repetition_maximum">1</a>. These formulas are based on
    different assumptions about how strength changes as the number of repetitions increases <a
    href="https://en.wikipedia.org/wiki/One-repetition_maximum">1</a>.

</WelcomeItem></template>
