<script>
    export let data
</script>

<!-- <h1>{data.title}</h1> -->

<!-- <pre>
    {JSON.stringify(data,null, 2)}
</pre> -->

<main>
	<div class="card-container">
		<span class="pro">{data.label}</span>
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img class="round" src="{ data.zenit.url }" alt="profile photo" />
		<h3>{data.title}</h3>
		<p>{ data.bio[0].text }<br/></p>
        <h6>{data.locatie}</h6>
		<div class="buttons">
			<button class="primary">{data.message}</button>
			<button class="primary ghost"> {data.follow}</button>
		</div>
		<div class="skills">
			<h6>{data.skill}</h6>
			<ul>
				<li>{ data.skills[0].text}</li>
			</ul>
		</div>
	</div>
</main>