<script>
	let members = [
		{
			label: 'Directors',
			members: [
				{
					name: 'Darren Tan',
					role: 'President & Founder',
					img: 'https://www.onepwaa.org/assets/img/darren-tan_13.jpg'
				},
				{
					name: 'Sarah Swea',
					role: 'Vice-President',
					img: 'https://www.onepwaa.org/assets/img/2-sarahswea-1_1.jpg'
				},
				{
					name: 'Elaine Zhu',
					role: 'CEO',
					img: 'https://www.onepwaa.org/assets/img/web-elainezhu.jpg'
				},
				{
					name: 'Mr. Darren Lim',
					role: 'Faculty Advisor',
					img: 'https://www.onepwaa.org/assets/img/mr-darren-lim_7.jpg'
				},
				{
					name: 'Roshni Ruben',
					role: 'Director of Bloggers',
					img: 'https://www.onepwaa.org/assets/img/blogger-roshni-ruben.jpg'
				},
				{
					name: 'Manaam Raza',
					role: 'Director of Scholars',
					img: 'https://www.onepwaa.org/assets/img/scholar-manaamraza.jpg'
				},
				{
					name: 'Hui Yen Lim',
					role: 'Director of Design',
					img: 'https://www.onepwaa.org/assets/img/designer-huiyenlem.jpg'
				},
				{
					name: 'Arsh Shrivastava',
					role: 'Director of Events & Partnerships',
					img: 'https://www.onepwaa.org/assets/img/scholar-arsh-shrivastava.jpeg'
				},
				{
					name: 'Sam Poder',
					role: 'Webmaster',
					img: 'https://www.onepwaa.org/assets/img/designer-sampoder.jpg'
				}
			]
		},
		{
			label: 'Scholars',
			members: [
				{
					name: 'Stephanie Komala',
					role: 'Junior Director',
					img: 'https://www.onepwaa.org/assets/img/scholar-stephaniekomala-1.jpg'
				},
				{
					name: 'Advit Garg',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/scholar-advitgarg.jpg'
				},
				{
					name: 'Manas Kapur',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/scholar-manas-kapur.jpg'
				},
				{
					name: 'Manal Raza',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/scholar-manal-raza.jpeg'
				}
			]
		},
		{
			label: 'Designers',
			members: [
				{
					name: 'Abhiram Dasika',
					role: 'Junior Director',
					img: 'https://www.onepwaa.org/assets/img/scholar-stephaniekomala-1.jpg'
				},
				{
					name: 'Gabriella Sally',
					role: 'Junior Webmaster',
					img: 'https://www.onepwaa.org/assets/img/designer-abhiramdasika.jpg'
				},
				{
					name: 'Miguel Belen',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/designer-miguelbelen.jpg'
				},
				{
					name: 'Rhowan Ho',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/12-rhowanho_1.jpg'
				},
				{
					name: 'Dalia Ibrahim',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/blogger-daliaibrahim.jpeg'
				}
			]
		},
		{
			label: 'Events & Partnerships',
			members: [
				{
					name: 'Mehzad Chowdhury',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/peopleandculture-mehzadchowdhury.png'
				},
				{
					name: 'Oreoluwa Sofolaha',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/peopleandculture-oreoluwasofolahan.jpg'
				},
				{
					name: 'Manas Kapur',
					role: 'Contributor',
					img: 'https://www.onepwaa.org/assets/img/scholar-manas-kapur.jpg'
				}
			]
		}
	];
</script>
<div style="width: 100vw">
<div class="relative h-80">
	<div
		class="z-50 top-0 left-0 h-80 w-full absolute flex text-white items-center flex-col justify-center"
		style="background-image: linear-gradient(
      0deg,
      rgba(0, 0, 0, 0.55),
      rgba(0, 0, 0, 0.55)
    ),url('https://cloud-4er9w7ha5.vercel.app/0received_2675129871291122549667505451911559.jpeg');
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;"
	>
		<h1 class="text-6xl mb-2">This is</h1>
		<h1 class="text-8xl font-bold mb-3">Our Story</h1>
	</div>
	<img
		src="https://cloud-4er9w7ha5.vercel.app/0received_2675129871291122549667505451911559.jpeg"
		class=" h-80 w-full object-cover absolute top-0 left-0 z-20"
		alt="The OnePwaa Team"
	/>
</div>
<div class="mx-auto max-w-2xl">
	<p class="mt-6">
		OnePwaa is an international nonprofit dedicated to improving access to education among
		schoolchildren. Our mandate is to advocate for the concept and practice of collaborative
		learning principally through the World Scholar’s Cup (WSC) and other educational programs. We
		offer resources and services including but not limited to scholarship programs, debate camps,
		and study guides. We pledge to reinvest all profits obtained into the education of
		underprivileged communities internationally.
	</p>
	<p class="mt-4 mb-8">
		We pledge to offer our resources and services to all people—regardless of ethnicity, race,
		religion, socioeconomic status, gender identity and sexual orientation—undoubtedly committed to
		reducing systemic disadvantages in education.
	</p>

	{#each members as group}
		<h2 class="text-3xl font-bold my-5" style="grid-column: 1 / span 2">{group.label}</h2>
		<div class="pb-3 grid grid-cols-2 gap-5">
			{#each group.members as member}
				<div class="flex items-center">
					<img
						src={member.img}
						class="w-20 h-20 object-cover rounded-md object-cover mr-4"
						alt={member.name}
					/>
					<div>
						<h4 class="text-xl font-bold">{member.name}</h4>
						<h4 class="mb-1">{member.role}</h4>
					</div>
				</div>
			{/each}
		</div>
	{/each}
	<br />
	<br />
	<div></div>
</div>
</div>