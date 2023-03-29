<script>
  import Navigation from "../lib/components/Navigation.svelte";
  import PageHeader from "../lib/components/PageHeader.svelte";
  import Footer from "../lib/components/Footer.svelte";
  


	const logo_image="/Images/Logo.jpg";
	let links = [
		{
			href: "/",
			title: "Home",
			
		},
		{
			href:"/project",
			title:"Project",
		},
		{
			href:"/stakeholders",
			title:"Stakeholders",
		},
		{
			href:"/budget",
			title:"Budget",
		},
		{
			href: "/framework",
			title: "Framework",
			
		},
		{
			href: "/hosting",
			title: "Hosting",
			
		},
		{
			href: "/security",
			title: "Security",
			
		},
		{
			href: "/reference",
			title: "Reference",
			
		},
		{
			href: "/carbon",
			title: "CO2-- Tech",
			
		},
	];

</script>



<main >
	<header>
		<PageHeader {logo_image}/>
		<Navigation {links} />
		<hr>
	</header>



<slot />
<hr>
<footer>
	<Footer/>
</footer>
</main>

<style>
	
@import url("https://unpkg.com/@picocss/pico@latest/css/pico.classless.min.css");
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200&display=swap");

main {
  font-family: 'Poppins', sans-serif;
  width: 95%;
  margin:auto;
}


</style>
