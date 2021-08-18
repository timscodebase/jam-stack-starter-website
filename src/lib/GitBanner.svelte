<script>
  import Icon from 'svelte-awesome';
  import { faGithub } from '@fortawesome/free-brands-svg-icons';
</script>

<a href="https://github.com/timscodebase/jam-stack-starter" target="_blank" rel="nofollow onopener">
  <div class="grid">
    <Icon data={faGithub} scale={5}/>
    <p>Follow on Github</p>
  </div>
</a>

<style>
  .grid {
    --size: 300px;
    width: var(--size);
    height: var(--size);
    background-color: var(--highlight-light);
    position: absolute;
    top: calc(var(--size) * -0.75666667);
    right: calc(var(--size) * -0.50666667);
    transform: rotate(45deg);
    border-bottom: 4px solid var(--highlight-dark);
    display: grid;
    padding-top: 1em;
    place-items: center;
    color: var(--black);
    font-size: 1.5em;
    font-weight: 300;
  }

  p {
    margin: 0;
  }
</style>