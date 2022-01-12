
<svelte:head>
	<title>Home</title>
</svelte:head>

<script>
	if (process.browser) {
			if(getCookie("hidden-event-banner") == "true"){
				document.getElementById("event-banner").style.display = "none";
			}
	}
</script>

<div class="flex flex-col min-h-screen">
	<div class="bg-blue-900 py-3 px-4 text-white font-bold flex items-center" id="event-banner">
		<h3 class="flex-grow">Join Us On 29th January for the What The Pwaa! Debate Tournament</h3>
		<h3 class="text-5xl close font-normal">+</h3>
	</div>
	<div class="bg-gray-900 py-4 px-4">
		<img src="img/onepwaa-logo-black.png" class="h-10" alt="OnePwaa" />
	</div>
	<div class="flex flex-col flex-grow" id="menu">
		<div class="bg-theme-red section">
			<h2 class="home-heading-text flex-grow">Study Guides</h2>
			<h2 class="home-heading-text chevorn italic">&gt;&gt;&gt;</h2>
		</div>
		<div class="bg-theme-green section">
			<h2 class="home-heading-text flex-grow">Deep Dives</h2>
			<h2 class="home-heading-text chevorn">&gt;&gt;&gt;</h2>
		</div>
		<div class="bg-theme-peach section">
			<h2 class="home-heading-text flex-grow">Strategy</h2>
			<h2 class="home-heading-text chevorn">&gt;&gt;&gt;</h2>
		</div>
		<div class="bg-theme-purple section">
			<h2 class="home-heading-text flex-grow">Humans of WSC</h2>
			<h2 class="home-heading-text chevorn">&gt;&gt;&gt;</h2>
		</div>
		<div class="bg-theme-blue section">
			<h2 class="home-heading-text flex-grow">About Us</h2>
			<h2 class="home-heading-text chevorn">&gt;&gt;&gt;</h2>
		</div>
	</div>
</div>