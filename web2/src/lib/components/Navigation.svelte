<script>
	export let links;
  </script>
  
  <nav  >
	<ul >
	  {#each links as link}
		<li>
		  <a href={link.href} title={link.title}>{link.title}</a>
		</li>
	  {/each}
	</ul>
  </nav>
  
  <style>
	nav {
		display: grid;
	  grid-template-columns: repeat(4, 1fr);
	  grid-auto-rows: auto;
	  grid-gap: 10px;
	  margin: auto;
	  width: 95%;
	}

  
	nav ul {
	  padding: 0;
	  list-style-type: none;
	  margin: 0;
	}
  

  
	a {
	  font-weight: 400;
	  text-transform: uppercase;
	  text-decoration: none;
	  color: #d3a2a2;
	  transition: color 0.3s ease;
	}
  
	a:hover {
	  color: #dbf302;
	}
  
	ul {
	  list-style-type: none;
	  padding: 0;
	}
  
	li {
	  margin-bottom: 10px;
	}
  </style>
  