<script>
	let games = [
		[
			{
				name: 'Business Blueprint Bash',
				poster: '/events/1.png',
				posterLowRes: '/events/1.png',
				date: '2nd Feburary 2024',
				link: 'https://forms.gle/DadbZveBnERQMoV88'
			},
			{
				name: 'Clash of Minds: Business Edition',
				poster: '/events/2.png',
				posterLowRes: '/events/2-lowres.png',
				date: '2nd Feburary 2024',
				link: 'https://forms.gle/JdbyafTD5ZWeuokz8'
			},
			{
				name: 'Trade Trivia Tournament - Paper Trading',
				poster: '/events/7.png',
				posterLowRes: '/events/7.png',
				date: '2nd Feburary 2024',
				link: 'https://forms.gle/UAQT52r71c1omieN9'
			},
			{
				name: 'BizQuiz Bonanza',
				poster: '/events/10.png',
				posterLowRes: '/events/10.png',
				date: '2nd Feburary 2024',
				link: 'https://forms.gle/NbCY7H8c81Veqc1i6'
			},
			{
				name: 'Market Mingle',
				poster: '/events/6.png',
				posterLowRes: '/events/6.png',
				date: '2nd & 3rd Feburary 2024',
				link: 'https://forms.gle/SpPTdcfd23LteMJ66'
			}
		],
		[
			{
				name: 'MIT Ted Talks',
				poster: '/events/4.png',
				posterLowRes: '/events/4.png',
				date: '3rd Feburary 2024',
				link: 'https://docs.google.com/forms/d/e/1FAIpQLSd6HwpP8L_0cBlm_JDe9oJS_7FtmzoEq7ZoWNJPrBlU1nwouA/viewform?usp=sf_link'
			},
			{
				name: '1-Min Games',
				poster: '/events/5.png',
				posterLowRes: '/events/5.png',
				date: '3rd Feburary 2024',
				link: 'https://forms.gle/MpHwjWPviC4YQ7KRA'
			},
			{
				name: 'Biz Hunt',
				posterLowRes: '/events/3.png',
				poster: '/events/3.png',
				date: '3rd Feburary 2024',
				link: 'https://forms.gle/HP5Wr3StTnMPpw2R7'
			},
			{
				name: 'PublicityPulse: The PR Event',
				poster: '/events/8.png',
				posterLowRes: '/events/8.png',
				date: '3rd Feburary 2024',
				link: 'https://forms.gle/hbXeBrteoUGnkd4G7'
			},
			{
				name: 'Design Dual(logo/ tagline/ brand ad)',
				poster: '/events/9.png',
				posterLowRes: '/events/9.png',
				date: '3rd Feburary 2024',
				link: 'https://forms.gle/u2vn13h8XNzfrxH56'
			}
		]
	];
</script>

<section id="event">
	<div class="container">
		<div class="row">
			<div class="col-sm-12 col-md-9">
				<div id="event-carousel" class="carousel slide" data-interval="false">
					<h2 class="heading">Events List</h2>
					<a class="even-control-left" href="#event-carousel" data-slide="prev"
						><i class="fa fa-angle-left"></i></a
					>
					<a class="even-control-right" href="#event-carousel" data-slide="next"
						><i class="fa fa-angle-right"></i></a
					>
					<div class="carousel-inner">
						{#each games as game, i}
							<div class="item {i === 0 ? 'active' : ''}">
								<div class="row">
									{#each game as event}
										<div class="col-sm-4">
											<a href={event.link} class="single-event">
												<img class="img-responsive" src={event.poster} alt={event.name} />
												<h4>{event.name}</h4>
												<p>{event.date}</p>
											</a>
										</div>
									{/each}
								</div>
							</div>
						{/each}
					</div>
					<!-- <button> -->
					<div class="crausel-btn-group">
						<a class="btn btn-info" href="#event-carousel" data-slide="prev"
							><i class="fa fa-angle-left"></i></a
						>
						<a class="btn btn-info" href="#event-carousel" data-slide="next"
							><i class="fa fa-angle-right"></i></a
						>
					</div>
					<!-- </button> -->
				</div>
			</div>
			<div class="guitar">
				<img class="img-responsive" src="images/guitar.png" alt="guitar" />
			</div>
		</div>
	</div>
</section>

<style>
	.crausel-btn-group {
		display: flex;
		/* justify-content: space-around; */
		gap: 1rem;
		justify-content: center;
		max-width: 100%;
		margin: 2rem 0;
	}
</style>
