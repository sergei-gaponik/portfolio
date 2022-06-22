<template>
  <div class="container">
    <h2>Referenzen</h2>
    <div class="flex-v">
      <reference 
        v-for="(reference, i) in references" 
        :key="i" 
        :reference="reference"
      />
    </div>
  </div>
</template>

<script>
export default {
  data(){

    const references = [
      {
        title: "Hedo Parfümerie & Kosmetik",
        content: [
          "Entwicklung und Bereitstellung eines Shopify-Webshops",
          "Individuelle Lösungen zur Absatzoptimierung wie dynamische Preisanpassung"
        ]
      },
      {
        title: "EMPHI GmbH",
        content: [
          "Beteiligung an der technischen Umsetzung einer Software zum Auswerten von Börsendaten",
          "Konzeptionierung und Entwicklung einer Webanwendung für Personalmanagement"
        ]
      },
      {
        title: "Weber & Partner GmbH",
        content: [
          "Entwicklung einer Webanwendung für die Datenmodellierung und -darstellung eines Planungs-Handbuches"
        ]
      }
    ]

    return {
      references
    }
  }
}
</script>