<template>
  <div class="container">
    <p class="fs-2 p-2 text-center">活動</p>
    <card-component :content="card1" />
    <br />
    <card-component :content="card2" />
    <br />
    <card-component :content="card3" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import CardComponent, { Card } from "@/components/CardComponent.vue";

export default defineComponent({
  name: "AboutView",
  components: {
    CardComponent,
  },
  setup() {
    const card1 = {
      title: "地域の施設訪問、レクリエーション",
      message:
        "&emsp;老人介護施設や病院で、利用者・患者さんにレクリエーションを行っています。生き生きと、楽しく、認知症予防にもなる内容を心がけています。",
      image: "p2.jpg",
    } as Card;
    const card2 = {
      title: "認知症カフェ",
      message:
        "&emsp;あま市 ○○、△△にて、年数回ずつ認知症カフェを開いています。",
      image: "p3.jpg",
    } as Card;
    const card3 = {
      title: "あま市民病院でのボランティア",
      message:
        "<div>&ensp;ワクチン接種会場でのボランティア</div><div>&ensp;医療者に、使い捨てエプロン作成</div><div>&ensp;病棟でのレクリエーション</div>",
      image: "p4.jpg",
    } as Card;
    return {
      card1,
      card2,
      card3,
    };
  },
});
</script>
