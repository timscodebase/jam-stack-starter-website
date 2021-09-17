<script>
  import GitBanner from "$lib/GitBanner.svelte";
</script>

<!-- <GitBanner /> -->
<header>
  <h1>Jamstack Starter</h1>
  <h2>The easiest way to get started on your next web project</h2>
<p>This CLI will walk you though your first project, and get you setup with the tools you need to build a modern web app. There are no prerequisites, and no configuration. Just run the command and you're ready to go.</p>
</header>

<main>
  <pre>npm i -g jam-stack-starter

jam-stack-starter</pre>

  <div class="image-wrapper">
    <img src="framework.png" alt="Framework">
  </div>

  <div class="image-wrapper">
    <img src="choice.png" alt="Choices">
  </div>
</main>

<footer>
  <p>
    Jamstack Starter &copy; 2021</p>
  <p>
    Created by <a class="green" href="https://timsmith.tech" target="_blank" rel="nofollow onopener">Tim Smith</a>
  </p>
  <p>
    <a class="purple" href="https://github.com/timscodebase/jam-stack-starter" target="_blank" rel="nofollow onopener">Github</a>
  </p>
</footer>

<style>
  .image-wrapper {
    width: 60%;
    min-width: 350px;
    padding: 1rem 0;
    margin: 2rem 0 1rem 0;
    background-color: #0b273a;
    border-radius: 2rem;
    padding: 1rem 0.25rem 0 0.25rem;
    color: var(--white);
    overflow: hidden;
    border: 1px solid var(--highlight-light);
  }
  .image-wrapper:first-of-type {
    border: 1px solid var(--highlight-dark);
  }

  h1 {
    position: relative;
    font-size: 3.5rem;
    text-align: center;
    font-weight: 300;
    background: linear-gradient(45deg, var(--highlight-light), var(--highlight-dark));
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-stroke: 4px transparent;
    color: var(--white);
  }

  img {
    max-width: 100%;
    height: auto;
    object-fit: contain;
  }

  main {
    margin-top: 2rem;
    display: grid;
    place-items: center;
  }

  header {
    margin-top: 4rem;
    display: grid;
    place-items: center;
  }

  header p, header h2 {
      margin: 1rem 10vw;
    }

  pre {
    margin: 2rem 0;
    border-radius: 2rem;
    padding: 1rem 2rem;
    color: var(--white);
    border: 1px solid #24BF00;
    background: var(--black);
    transition: all 0.2s ease;
    animation: spin 4s infinite linear;
  }

  a {
    font-weight: 300;
    color: var(--white);
    transition: all 0.2s ease;
    animation: a-spin 4s infinite linear;
  }

  footer {
    padding: 2rem;
    font-weight: 200;
    line-height: 1.5;
    text-align: center;
  }

  @keyframes a-spin {
    0% {
      text-shadow: -5px 2px 10px var(--highlight-light),
                  5px -2px 10px var(--highlight-dark);
    }
    25% {
      text-shadow: -5px -2px 10px var(--highlight-light),
                  5px 2px 10px var(--highlight-dark);
    }
    50% {
      text-shadow: 5px -2px 10px var(--highlight-light),
                  -5px 2px 10px var(--highlight-dark);
    }
    75% {
      text-shadow: 5px 2px 10px var(--highlight-light),
                  -5px -2px 10px var(--highlight-dark);
    }
    100% {
      text-shadow: -5px 2px 10px var(--highlight-light),
                  5px -2px 10px var(--highlight-dark);
    }
  }

  @keyframes spin {
    0% {
      box-shadow: -20px 10px 50px var(--highlight-light),
                  20px -5px 50px var(--highlight-dark);
    }
    25% {
      box-shadow: 20px 10px 50px var(--highlight-light),
                  -30px -5px 50px var(--highlight-dark);
    }
    50% {
      box-shadow: 20px -5px 50px var(--highlight-light),
                  -20px 5px 50px var(--highlight-dark);
    }
    75% {
      box-shadow: -20px -5px 50px var(--highlight-light),
                  20px 5px 50px var(--highlight-dark);
    }
    100% {
      box-shadow: -20px 5px 50px var(--highlight-light),
                  20px -5px 50px var(--highlight-dark);
    }
  }
</style>

