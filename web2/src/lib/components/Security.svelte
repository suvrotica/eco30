<script>
    import { onMount } from 'svelte';
    import SvelteMarkdown from 'svelte-markdown';
    let source = '';
  
    onMount(async () => {
      const response = await fetch('security.md');
      source = await response.text();
    });
  </script>
  
  <SvelteMarkdown {source} />