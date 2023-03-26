<script>
	export let links;
  </script>
  
  <nav   >
	<ul class="navbar">
	  {#each links as link}
		<li class="link">
		  <a href={link.href} title={link.title}>{link.title}</a>
		</li>
	  {/each}
	</ul>
  </nav>
  
  <style>
	.navbar {
		
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-flow: row;
  grid-auto-rows: 20px;
  width: 95%;
  margin:auto;
}

.link {
  grid-row-start: span 1;
  width: 100%;
}


.link:nth-child(5) {
  grid-row-start: 2;
}

.link:nth-child(9) {
  grid-row-start: 3;
}


  
	a {
	  font-weight: 300;
	  text-transform: full-width;
	  text-decoration: none;
	  color: #e0dcb0;
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
  