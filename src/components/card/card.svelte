<script lang="ts">
	export let title: string;
	export let attrList: any[];
	export let buttonName: string = "Detalhes";
</script>

<div class="card card-side bg-base-100 bg-neutral p-2 shadow-md hover:bg-neutral-focus">
	<figure><img class="max-h-48" src="default-whey-img.png" alt="Whey" /></figure>
	<div class="card-body cursor-default">
		<h2 class="card-title">{title}</h2>
		{#each attrList as attr, i}
			<div>{attr}</div>
		{/each}
		<div class="card-actions justify-end">
			<button class="btn btn-primary">{buttonName}</button>
		</div>
	</div>
</div>
