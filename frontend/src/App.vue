<script setup>
import Tuerchen from "@/components/Tuerchen.vue";
</script>

<template>
  <div class="tuerchen-container">
    <Tuerchen text="Guten Morgen! Heute beginnt der Advent – Zeit für Kekse und Kerzen."
              tuerchen-nummer="1"/>
    <Tuerchen text="Ein schöner Tag für einen Spaziergang im Winterwald." tuerchen-nummer="2"/>
    <Tuerchen text="Heute gibt es eine kleine Überraschung für dich!" tuerchen-nummer="3"/>
    <Tuerchen text="Zeit, sich eine Tasse heißen Kakao zu gönnen." tuerchen-nummer="4"/>
    <Tuerchen text="Weihnachtliche Musik bringt heute gute Laune." tuerchen-nummer="5"/>
    <Tuerchen text="Heute kannst du ein kleines DIY-Weihnachtsgeschenk basteln."
              tuerchen-nummer="6"/>
    <Tuerchen text="Ein bisschen Winterzauber gefällig? Kerzen an!" tuerchen-nummer="7"/>
    <Tuerchen text="Zeit, einen Weihnachtsfilm zu schauen." tuerchen-nummer="8"/>
    <Tuerchen text="Heute darfst du dir etwas Leckeres backen." tuerchen-nummer="9"/>
    <Tuerchen text="Ein kleiner Spaziergang durch die festlich geschmückte Stadt."
              tuerchen-nummer="10"/>
    <Tuerchen text="Heute ist ein perfekter Tag für Plätzchen verzieren." tuerchen-nummer="11"/>
    <Tuerchen text="Weihnachtskarten schreiben für Freunde und Familie." tuerchen-nummer="12"/>
    <Tuerchen text="Heute kannst du ein bisschen Weihnachtsdeko basteln." tuerchen-nummer="13"/>
    <Tuerchen text="Zeit für eine gemütliche Leseecke mit Weihnachtsgeschichten."
              tuerchen-nummer="14"/>
    <Tuerchen text="Heute gibt es eine kleine Überraschung im Adventskalender."
              tuerchen-nummer="15"/>
    <Tuerchen text="Ein schöner Moment, um Weihnachtslieder zu singen." tuerchen-nummer="16"/>
    <Tuerchen text="Heute darfst du dir etwas Gutes tun und entspannen." tuerchen-nummer="17"/>
    <Tuerchen text="Zeit, eine kleine Weihnachtsbotschaft zu verschicken." tuerchen-nummer="18"/>
    <Tuerchen text="Heute gibt es Glühwein oder heißen Apfelsaft zum Aufwärmen."
              tuerchen-nummer="19"/>
    <Tuerchen text="Kleine Weihnachtsdeko für dein Zuhause basteln." tuerchen-nummer="20"/>
    <Tuerchen text="Heute ist ein Tag, um schöne Erinnerungen zu teilen." tuerchen-nummer="21"/>
    <Tuerchen text="Zeit, ein kleines Weihnachtsrätsel zu lösen." tuerchen-nummer="22"/>
    <Tuerchen text="Heute darfst du einfach die Adventsstimmung genießen." tuerchen-nummer="23"/>
    <Tuerchen text="Frohe Weihnachten! Heute endet der Advent – genieße den Tag."
              tuerchen-nummer="24"/>
  </div>
</template>

<style scoped>

.tuerchen-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, auto));
  gap: 20px;
  justify-content: center;
}
</style>
