<script>
    import { onMount } from 'svelte';
    
    let darkMode;
    let buttonText;
    
    function toggleTheme() {
      darkMode = !darkMode;
      localStorage.setItem('theme', darkMode ? 'dark' : 'light');
      applyTheme();
    }
    
    function applyTheme() {
      document.documentElement.setAttribute('data-theme', darkMode ? 'dark' : 'light');
      buttonText = darkMode ? 'Light Mode' : 'Dark Mode';
    }
    
    onMount(() => {
      darkMode = localStorage.getItem('theme') === 'dark';
      applyTheme();
    });
  </script>


  
  <style>
    /* Light theme styles */
    :root[data-theme='light'] {
      background-color: white;
      color: black;
    }
  
    /* Dark theme styles */
    :root[data-theme='dark'] {
      background-color: black;
      color: white;
    }

  </style>
    
  <button on:click={toggleTheme}>{buttonText}</button>
  