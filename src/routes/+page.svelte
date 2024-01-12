<script>
  let noticias = [
      {
          titulo: 'Notícia 1',
          data: '2022-10-01',
          conteudo: 'Conteúdo da notícia 1'
      },
      {
          titulo: 'Notícia 2',
          data: '2022-09-15',
          conteudo: 'Conteúdo da notícia 2'
      },
      {
          titulo: 'Notícia 3',
          data: '2022-08-25',
          conteudo: 'Conteúdo da notícia 3'
      }
  ];
</script>

<main>
  <h1>Notícias</h1>

  <article>
    <h2>{noticias[0].titulo}</h2>
    <p>{noticias[0].data}</p>
    <p>{noticias[0].conteudo}</p>
  </article>

  <ul>
    {#each noticias.slice(1) as noticia}
      <li>
        <h3>{noticia.titulo}</h3>
        <p>{noticia.data}</p>
      </li>
    {/each}
  </ul>
</main>

<style>
  main {
    max-width: 600px;
    margin: 0 auto;
  }

  article {
    margin-bottom: 20px;
  }

  h1 {
    font-size: 24px;
    margin-bottom: 10px;
  }

  h2 {
    font-size: 20px;
    margin-bottom: 5px;
  }

  h3 {
    font-size: 18px;
    margin-bottom: 5px;
  }

  p {
    font-size: 14px;
    margin-bottom: 5px;
  }
</style>