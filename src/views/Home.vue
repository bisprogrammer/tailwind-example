<template>
  <div class="font-sans">
    <Header />
    <Promo />
    <Advantages :items="advantages" />
    <History :items="history" />
    <Questions />
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header";
import Promo from "../components/Promo";
import Advantages from "../components/Advantages";
import History from "../components/History";
import Questions from "../components/Questions";
import Footer from "../components/Footer";

export default {
  name: 'Home',
  components: {
    Header,
    Promo,
    Advantages,
    History,
    Questions,
    Footer
  },
  data() {
    return {
      advantages: [
        {
          id: 1,
          image: "/img/advantage1.svg",
          count: 482,
          text: "Организаций поддержки по Российской Федерации"
        },
        {
          id: 2,
          image: "/img/advantage2.svg",
          count: 5240,
          text: "Оказано услуг государственной поддержки"
        },
        {
          id: 3,
          image: "/img/advantage3.svg",
          count: 1360,
          text: "Зарегестрировано участников проекта"
        }
      ],
      history: [
        {
          id: 1,
          avatar: "/img/image1.svg",
          title: 'Пекарня “Русские традиции”',
          blockquote: "Как говорит сам Владимир: «мне хотелось, чтобы все узнали, что такое русская кухня», «обьяснить, что она жива».",
          text: "Чтобы мини-пекарня стала рентабельным бизнесом, необходимы строгие расчеты, учет рисков и перспектив, анализ рынка, налаживание сбыта."
        },
        {
          id: 2,
          avatar: "/img/image2.svg",
          title: 'Автомастерская',
          blockquote: "Первые дни независимости. Когда не нужно рано вставать, когда не нужно отпрашиваться, что бы успеть съездить в магазин, когда удобно.",
          text: "Встреча в городе Н с моими будущими партнерами была плодотворной. Я не смог заснуть до пяти утра – не потому что не спалось, но потому что мысли о будущих перспективах просто взрывали мой мозг."
        },
        {
          id: 3,
          avatar: "/img/image3.svg",
          title: 'Салон красоты “Эмират”',
          blockquote: "Когда же появилась возможность открыть свой бизнес, я рассматривала различные варианты, изучала всевозможные направления."
        }
      ]
    }
  }
}
</script>
