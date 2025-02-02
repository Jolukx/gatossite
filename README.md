<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Meta tag para responsividade -->
    <title>AppFotosDeGatos</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
      /* Estilo global */
      body {
        font-family: 'Roboto', Arial, sans-serif;
        line-height: 1.6;
        margin: 0;
        padding: 0;
        background: url('https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg') center/cover no-repeat, rgba(255, 255, 255, 0.9);
        background-blend-mode: overlay;
        color: #333;
        text-align: center;
      }

      /* Cabeçalho principal */
      h1 {
        color: #444;
        margin-top: 20px;
      }

      /* Links */
      a {
        color: #0066cc;
        text-decoration: none;
      }

      a:hover {
        text-decoration: underline;
      }

      /* Seções */
      section {
        margin: 20px auto;
        padding: 20px;
        background: rgba(255, 255, 255, 0.8);
        border: 1px solid #ddd;
        border-radius: 8px;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        max-width: 600px;
      }

      /* Imagens */
      img {
        max-width: 100%;
        height: auto;
        margin: 10px 0;
        border-radius: 8px;
      }

      /* Listas */
      ul, ol {
        padding-left: 0;
        list-style-position: inside;
        text-align: left;
        margin: 10px auto;
        display: inline-block;
      }

      /* Formulário */
      form {
        margin-top: 20px;
        display: flex;
        flex-direction: column;
        gap: 15px;
        align-items: center;
      }

      input[type="text"], button {
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ddd;
        border-radius: 4px;
        width: 80%;
        max-width: 300px;
      }

      button {
        background-color: #28a745;
        color: white;
        border: none;
        cursor: pointer;
      }

      button:hover {
        background-color: #218838;
      }

      /* Rodapé */
      footer {
        text-align: center;
        padding: 10px;
        background: #444;
        color: white;
        margin-top: 20px;
      }

      /* Responsividade para dispositivos móveis */
      @media screen and (max-width: 768px) {
        section {
          padding: 10px;
          margin: 10px;
          width: 90%;
        }

        h1 {
          font-size: 1.5em;
        }

        h2 {
          font-size: 1.2em;
        }

        input[type="text"], button {
          width: 90%;
        }
      }

      @media screen and (max-width: 480px) {
        h1 {
          font-size: 1.2em;
        }

        h2 {
          font-size: 1em;
        }

        section {
          width: 95%;
        }

        button {
          padding: 12px;
          font-size: 18px;
        }
      }
    </style>
  </head>
  <body>
    <main>
      <h1>AppFotosDeGatos</h1>
      <section>
        <h2>Fotos de Gatos</h2>
        <p>Todo mundo ama <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">gatinhos fofos</a> na internet!</p>
        <p>Veja mais <a target="_blank" href="https://freecatphotoapp.com">fotos de gatos</a> na nossa galeria.</p>
        <a href="https://freecatphotoapp.com">
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="Um fofo gato laranja deitado de costas.">
        </a>
      </section>
      <section>
        <h2>Listas de Gatos</h2>
        <h3>Coisas que os gatos amam:</h3>
        <ul>
          <li>erva-de-gato</li>
          <li>pontos de laser</li>
          <li>lasanha</li>
        </ul>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="Uma fatia de lasanha em um prato.">
          <figcaption>Os gatos <em>amam</em> lasanha.</figcaption>
        </figure>
        <h3>As 3 principais coisas que os gatos odeiam:</h3>
        <ol>
          <li>tratamento de pulgas</li>
          <li>trovão</li>
          <li>outros gatos</li>
        </ol>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Cinco gatos olhando ao redor de um campo.">
          <figcaption>Os gatos <strong>odeiam</strong> outros gatos.</figcaption>
        </figure>
      </section>
      <section>
        <h2>Formulário de Gatos</h2>
        <form action="https://freecatphotoapp.com/submit-cat-photo">
          <fieldset>
            <legend>Seu gato é doméstico ou de rua?</legend>
            <label><input id="domestico" type="radio" name="domestico-ou-rua" value="domestico" checked> Doméstico</label>
            <label><input id="rua" type="radio" name="domestico-ou-rua" value="rua"> De rua</label>
          </fieldset>
          <fieldset>
            <legend>Qual é a personalidade do seu gato?</legend>
            <input id="amoroso" type="checkbox" name="personalidade" value="amoroso" checked> 
            <label for="amoroso">Amoroso</label>
            <input id="preguicoso" type="checkbox" name="personalidade" value="preguicoso"> 
            <label for="preguicoso">Preguiçoso</label>
            <input id="energetico" type="checkbox" name="personalidade" value="energetico"> 
            <label for="energetico">Energético</label>
          </fieldset>
          <input type="text" name="urlfotogato" placeholder="Insira a URL da foto do seu gato" required>
          <button type="submit">Enviar</button>
        </form>
      </section>
    </main>
    <footer>
      <p>
        Sem Direitos Autorais - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
      </p>
    </footer>
  </body>
</html>
