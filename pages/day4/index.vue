<template>
  <div>
    <hero />
    <mission />
    <results :items="results.items" />
    <features />
    <business />
    <member />
    <update :items="update.items" />
    <recruit />
    <company />
  </div>
</template>

<script>
import Hero from "~/components/top/Hero.vue"
import Mission from "~/components/top/Mission.vue"
import Results from "~/components/top/Results.vue"
import Features from "~/components/top/Features.vue"
import Business from "~/components/top/Business.vue"
import Member from "~/components/top/Member.vue"
import Update from "~/components/top/Update.vue"
import Recruit from "~/components/top/Recruit.vue"
import Company from "~/components/top/Company.vue"

export default {
  components: {
    Hero,
    Mission,
    Results,
    Features,
    Business,
    Member,
    Update,
    Recruit,
    Company
  },
  data() {
    return {
      // ポートフォリオ
      results: {
        items: [
          {
            url: "https://www.kikagaku.co.jp",
            img_url: require("~/assets/img/front/portfolio/image1.jpg"),
            img_alt:
              "Preferred Networks社提供のChainerチュートリアル制作に協力",
            title:
              'Preferred Networks社提供の<span class="br__pc"></span>Chainerチュートリアル制作に協力'
          },
          {
            url: "#",
            img_url: require("~/assets/img/front/portfolio/image2.jpg"),
            img_alt: "メルカリ社の経営層向けAI研修の実施",
            title:
              'メルカリ社の経営層向けAI研修の<span class="br__pc"></span>実施'
          },
          {
            url: "#",
            img_url: require("~/assets/img/front/portfolio/image3.jpg"),
            img_alt: "ABEJA社とアセスメント人材育成コースを共同制作",
            title:
              'ABEJA社とアセスメント人材育成<span class="br__pc"></span>コースを共同制作'
          }
        ]
      },

      // キカガクブログ
      update: {
        items: [
          {
            url: "#",
            img_url: require("~/assets/img/sample/blog1.jpg"),
            img_alt:
              "ダミーテキスト。タイトルが入ります。タイトルが入ります...",
            title: "ダミーテキスト。タイトルが入ります。タイトルが入ります..."
          },
          {
            url: "#",
            img_url: require("~/assets/img/sample/blog2.jpg"),
            img_alt:
              "ダミーテキスト。タイトルが入ります。タイトルが入ります...",
            title: "ダミーテキスト。タイトルが入ります。タイトルが入ります..."
          },
          {
            url: "#",
            img_url: require("~/assets/img/sample/blog3.jpg"),
            img_alt:
              "ダミーテキスト。タイトルが入ります。タイトルが入ります...",
            title: "ダミーテキスト。タイトルが入ります。タイトルが入ります..."
          }
        ]
      }

    }
  }
}
</script>