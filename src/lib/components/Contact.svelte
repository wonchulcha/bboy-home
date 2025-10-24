<script>
  import Header from "./Header.svelte";
  import Footer from "./Footer.svelte";
</script>

<Header />

<main class="container">
  <h2>최고의 무대를 선사하겠습니다.</h2>
  <div class="contact">
    <figure class="map">
      <iframe
        title="빅보이 스튜디오"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d6310.724165890653!2d127.03727835082361!3d37.73464888798203!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357cc74aeba7ca93%3A0xb545b95d09aa0d2!2z7ZWc7IaU6rO17J247KSR6rCc7IKs!5e0!3m2!1sko!2skr!4v1761298355195!5m2!1sko!2skr"
        width="100%"
        height="450"
        style="border:0;"
        allowfullscreen={true}
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </figure>
    <address>
      <p>경기도 의정부시 범골로 123번길 11, 3층<br />빅브라더 스튜디오</p>
      <p>
        Email:
        <a href="mailto:bbrother@gmail.com">bbrother@gmail.com</a>
      </p>
      <p>
        Tel:
        <a href="tel:031-000-0000">031-000-0000</a> /
        <a href="tel:010-000-0000">010-000-0000</a>
      </p>
      <p>Fax: 031-000-0000</p>
    </address>
  </div>
</main>

<Footer />

<style>
  .contact {
    display: flex;
    gap: 75px;
    figure,
    address {
      width: 50%;
      font-style: normal;
    }
    address {
      p:not(:first-child) {
        margin-bottom: 5px;
      }
    }
    a {
      color: inherit;
    }
  }

  .container {
    background: #fff;
  }
</style>
