<script>
	export let links;
  </script>
  
  <nav>
	<ul>
	  <li>
		<strong>Carbon Credit Project</strong>
		<cite> - Eco30</cite>
	  </li>
	</ul>
	<ul>
	  {#each links as link}
		<li>
		  <a href={link.href} title={link.title}>{link.title}</a>
		</li>
	  {/each}
	</ul>
  </nav>
  
  <style>
	cite {
	  font-weight: 200;
	  color: #777;
	}
  
	strong {
	  font-weight: 600;
	  text-transform: uppercase;
	  color: #333;
	}
	
	nav {
	  margin: auto;
	  width: 95%;
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
  