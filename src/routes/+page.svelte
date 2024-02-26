<script lang="ts">
	import Icon from '$lib/Icon.svelte'

</script>
<svelte:head><base target="_blank" /></svelte:head>

<main class=container>
  <article>
    <header>
      <hgroup>
        <h2>Péter Bócz</h2>
        <p>web&nbsp;developer &bull; system&nbsp;administrator &bull; technical&nbsp;writer</p>
      </hgroup>
    </header>

    <section>
      <aside>
        <a href="https://github.com/boczpeter"><Icon icon=fa-brands:github double/></a>
        <a href="https://www.linkedin.com/in/peterbocz/"><Icon icon=fa6-brands:linkedin double/></a>
      </aside>

      <div>
        <Icon icon=iconamoon:star double title="Loves working with"/>
        <b>Linux</b>
        <b>Perl</b>
        <b>MySQL</b>
        <b><a href="https://kit.svelte.dev">SvelteKit</a></b>
        <b>CSS</b>
        <b>SVG</b>
        <Icon icon=iconamoon:star double title="Loves working with" cls=lg/>
      </div>

      <div>
        <Icon icon=noto:eyes double rot180 title="Interested in"/>
        <mark>#privacy</mark>
        <mark>#security</mark>
        <mark>#facts</mark>
        <Icon icon=solar:bicycling-bold double title=Cycling/>
        <Icon icon=twemoji:flag-european-union double title=EU/>
        <Icon icon=twemoji:flag-ukraine double title=Ukraine/>
        <Icon icon=noto:eyes double title="Interested in" cls=lg/>
      </div>
    </section>

    <footer>Made with
      <a href="https://kit.svelte.dev">SvelteKit</a>
        &bull;
      <a href="https://picocss.com">Pico.css</a>
        &bull;
      <a href="https://iconify.design">Iconify</a>
    </footer>
  </article>
</main>

<style>
  main {
    padding: 1rem;
    height: 100%;
    --border-radius: 3vw;
  }
  hgroup, p, article {
    margin-block: auto;
  }
  h2 {
    line-height: 1;
  }
  main, section, aside, div {
    display: flex;
    gap: 3vw;
    align-items: center;
  }
  section, main {
    flex-direction: column;
  }
  aside {
    gap: 10vw;
    line-height: 0;
  }
  aside a {
    font-size: 2rem;
  }
  mark {
    padding: 0.2em 0.5em;
    border-radius: 0.4em;
  }
  footer {
    font-size: 65%;
    line-height: 0;
  }

@media (max-width: 576px) {
	div {
		flex-wrap: wrap;
	}
}
</style>
