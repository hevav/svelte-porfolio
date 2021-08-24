<script>
	import Backplate from "./ui/Backplate.svelte";
	import Paper from "./ui/Paper.svelte";
	import IconLine from "./ui/IconLine.svelte";
</script>

<Backplate color="#567"/>
<main>
	<div class="container">
		<Paper logo="https://avatars.githubusercontent.com/u/14876058?v=4" header="/header.webp" color="#fafafa">
			<div class="desc">
				<div class="large">hevav.</div>
				<div class="medium">Software developer</div>
				<br>
				<div class="sideDesc">
					<div class="left">
						<IconLine icon="fas fa-map-marker-alt" text="Moscow, Russia"/>
						<IconLine icon="fas fa-code" text="Go, Svelte, Java"/>
						<a href="https://ely.su/"><IconLine icon="fas fa-briefcase" text="Elytrium"/></a>
						<a href="https://t.me/hevav"><IconLine icon="fab fa-telegram-plane" text="@hevav"/></a>
						<a href="https://vk.com/hevav"><IconLine icon="fab fa-vk" text="vk.com/hevav"/></a>
						<IconLine icon="fab fa-discord" text="hevav#9274"/>
					</div>
					<div class="right">
						<a href="https://github.com/Elytrium">
							<Paper color="#7f69a9">
								<div class="card">
									<div class="large medium name">Elytrium</div>
									<div class="name">Own game hosting platform</div>
								</div>
							</Paper>
						</a>
						<br>
						<a href="https://github.com/hevav/TchuBBak">
							<Paper color="#567">
								<div class="card">
									<div class="large medium name">TchuBBak</div>
									<div class="name">Simple Discord voice-bot</div>
								</div>
							</Paper>
						</a>
						<br>
						<a href="https://github.com/hevav/"><IconLine icon="fab fa-github" text="See more"/></a>
					</div>
				</div>
				<br>
			</div>
		</Paper>
		<br>
		<center><small>Portfolio website made using Svelte &lt;3 <br> &copy; 2021 hevav.dev</small></center>
	</div>
</main>

<style>
	main {
		width: 100vw;
		height: 100%;
		display: flex;
		justify-content: center;
		position: absolute;
	}

	.container {
		margin-top: 120px;
		padding: 1rem;
		max-width: 55rem;
		width: 95%;
	}

	.large {
		font-size: 3rem;
		font-weight: bold;
	}

	.name {
		color: white;
	}

	.medium {
		font-size: 1.5rem;
	}
	
	.sideDesc {
		display: flex;
		flex-direction: row;
	}

	.sideDesc > * {
		flex: 1;
	}

	.card {
		padding: 0.75rem 2rem;
	}

	.desc {
		padding: 2.5rem;
	}
	
	@media (max-width: 720px) {
		.sideDesc {
			flex-direction: column;
		}
	}
</style>