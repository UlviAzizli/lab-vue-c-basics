<script setup>
import { ref } from "vue";

const library = ref([
  {
    title: "The Night Circus",
    author: "Erin Morgenstern",
    description:
      "The Night Circus is a beautifully written novel that weaves a mesmerizing tale of magic, love, and destiny. The story revolves around a mysterious and enchanting circus that appears only at night, and the two young magicians, Celia and Marco, bound by a magical competition that could cost them everything. As they create increasingly wondrous and fantastical displays within the circus, their rivalry transforms into a deep and forbidden love. Erin Morgenstern's lyrical prose and imaginative storytelling make this a must-read for fans of fantasy and romance.",
  },
  {
    title: "Sapiens: A Brief History of Humankind",
    author: "Yuval Noah Harari",
    description:
      "Yuval Noah Harari's 'Sapiens' is a thought-provoking journey through the history of humankind, from the emergence of Homo sapiens in Africa to the present day. Harari explores the major revolutions that shaped our species, including the cognitive, agricultural, and industrial revolutions, and delves into how human societies and cultures have evolved over time. This book offers a compelling perspective on the forces that have shaped our world, from the development of language to the rise of empires. It challenges readers to question the narratives that underpin our beliefs about society and humanity's future.",
  },
  {
    title: "The Alchemist",
    author: "Paulo Coelho",
    description:
      "A timeless classic, 'The Alchemist' tells the story of Santiago, a shepherd boy who embarks on a quest to discover his personal legend. His journey takes him from Spain to the Egyptian desert as he seeks a hidden treasure and learns profound lessons about destiny, dreams, and the nature of the universe. Paulo Coelho's beautifully simple yet philosophical prose weaves together themes of self-discovery, fate, and the pursuit of one's dreams. 'The Alchemist' is a novel that inspires readers to follow their hearts and listen to the whispers of their souls as they seek their own paths in life.",
  },
]);
</script>

<template>
  <ul>
    <li v-for="book in library">
      <h3>Title : {{ book.title }},</h3>
      <i>Author : {{ book.author }},</i>
      <p>Description : {{ book.description }}</p>
    </li>
  </ul>
</template>

<style></style>
