<script>
  import Header from "./Header.svelte";
  import Footer from "./Footer.svelte";

  import { getNews } from "../../assets/news";

  export let params = {};
  console.log(params);
  console.log(getNews(Number(params.id)));
  let news = getNews(Number(params.id));
</script>

<Header />
<main class="container">
  <div class="main-header">
    <h2>{news.title}</h2>
    <p class="date">{news.date}</p>
    <img src={news.detailImgUrl} alt={news.title} />
  </div>
  <article>
    <p>
      {@html news.desc}
    </p>
  </article>
</main>
<Footer />

<style lang="scss">
  .main-header {
    h2 {
      margin-bottom: 10px;
    }
    .date {
      margin: 20px;
      font-size: 15px;
      color: #666;
    }
  }
  article {
    margin-top: 50px;
  }

  .container {
    background: #fff;
  }
</style>
