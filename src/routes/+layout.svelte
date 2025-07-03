<script lang="ts">
  import ogImage from '$lib/assets/og_image.jpg';
  import '../app.css';
  import { page } from '$app/stores';

  // реактивно обновляем fullHost при смене URL
  $: fullHost = $page.url.host;
</script>

<svelte:head>
  <title>Plinko</title>
  <!-- шрифты, стили и т.п. -->
  <meta property="og:url" content={`https://${fullHost}/`} />
  <meta property="og:image" content={ogImage} />
</svelte:head>

<slot />