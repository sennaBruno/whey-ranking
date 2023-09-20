<script>
	import Card from "../../components/card/card.svelte";

	let arrayWheyCards = [
		{ id: "J---aiyznGQ", title: "Whey Growth", attr: ["Listagem dos atributos do Whey", "Mais um atributo"] },
		{ id: "z_AbfPXTKms", title: "Whey Growth 2", attr: ["Listagem dos atributos do Whey 2"] },
		{ id: "OUtn3pvWmpg", title: "Whey Growth 3", attr: ["Listagem"] },
	];
</script>

<h1>Pagina de Rankeamento</h1>

<div class="container flex flex-col gap-4 p-4">
	{#each arrayWheyCards as wheyCards}
		<Card title={wheyCards.title} attrList={wheyCards.attr} />
	{/each}
</div>
