<script>
	// Dummy data for the list of articles
	let articles = [
		{
			id: '2020-05-11',
			title: 'From design thinking to design doing',
			description: 'How to build successful, emotionally resonant products.'
		},
		{
			id: '2019-08-21',
			title: 'Form vs Function',
			description: 'When is it okay for design to be weird?'
		},
		{
			id: '2018-05-12',
			title: 'The Power of Unfinished',
			description: 'How to create work that gets noticed.'
		}
		// Add more articles as needed
	];
</script>

<div class="header">
	<input type="search" placeholder="Search" />
	<button>Subscribe</button>
	<button>Sign in</button>
</div>

<div class="articles">
	{#each articles as article}
		<div class="article">
			<div class="date">{article.id}</div>
			<div class="content">
				<h2>{article.title}</h2>
				<p>{article.description}</p>
			</div>
		</div>
	{/each}
</div>

<style>
	.header {
		display: flex;
		justify-content: space-between;
		padding: 10px;
		background-color: #f0f0f0;
	}
	.header input[type='search'] {
		flex: 1;
		margin-right: 10px;
	}
	.articles {
		margin-top: 20px;
	}
	.article {
		display: flex;
		align-items: baseline;
		margin-bottom: 10px;
	}
	.date {
		width: 80px;
		color: grey;
		margin-right: 20px;
	}
	.content h2 {
		margin: 0;
		color: #333;
	}
	.content p {
		margin: 0;
		color: #666;
	}
</style>
