<script>
	import styles from "./style";
	import { Navbar, Billing, Hero } from "./components";
    import Stats from "./components/Stats.svelte";
    import Business from "./components/Business.svelte";
    import CardDeal from "./components/CardDeal.svelte";
    import Testimonial from "./components/Testimonial.svelte";
    import Clients from "./components/Clients.svelte";
    import Cta from "./components/CTA.svelte";
    import Footer from "./components/Footer.svelte";
</script>

<div class="bg-primary w-full overflow-hidden">
	<div class={`${styles.flexCenter} ${styles.paddingX}`}>
		<div class={`${styles.boxWidth}`}>
			<Navbar />
		</div>
	</div>

	<div class={`${styles.flexStart} bg-primary`}>
		<div class={`${styles.boxWidth}`}>
			<Hero />
		</div>
	</div>

	<div class={`bg-primary ${styles.flexStart} ${styles.paddingX}`}>
		<div class={`${styles.boxWidth}`}>
			<Stats />
			<Business />
			<Billing />
			<CardDeal />
			<Testimonial />
			<Clients />
			<Cta />
			<Footer />
		</div>
	</div>
</div>


<style>

</style>