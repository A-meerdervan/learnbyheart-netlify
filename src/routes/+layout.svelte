<script>
	import '../app.css'
	import Footer from './footer.svelte'

</script>

<div class="layout">
	<!-- <Header /> -->
	<div id=topblock>
		<!-- <p>this is the top block</p> -->
	</div>
	<main id=main>
		<!-- <PageTransition url={data.url}> -->
			<slot />
		<!-- </PageTransition> -->
	</main>

	<!-- <Footer /> -->
	<Footer />
</div>