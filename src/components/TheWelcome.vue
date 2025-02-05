<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'

const openReadmeInEditor = () => fetch('/__open-in-editor?file=README.md')
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Discord</template>
    Isso mesmo! Eu tenho um servidor do Discord! Fica logo ali, na
    <a href="https://dsc.gg/pipdpnd">Rua Discordancia, 000!</a>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Apps em Python, JS, TS, e mais</template>

    Sim, eu faço apps meus amigos! Uso a minha <a href="https://meta.ai">amiga</a> pra poder ter
    ideias ou me ajudar a debugar.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Me doa um café?</template>
    Bem, eu tenho um ko-fi, e se você pudesse me ajudar, por favor,
    <a href="https://bitly.cx/pipdpnd">doa pra mim?</a></WelcomeItem
  >
</template>
