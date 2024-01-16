<script>
	let games = [
		[
			{
				name: 'Business Blueprint Bash',
				poster: '/events/Business Blueprint Bash.jpg',
				posterLowRes: '/events/Business Blueprint Bash-lowres.jpg',
				date: '20th March 2021'
			},
			{
				name: 'Clash of Minds: Business Edition',
				poster: '/events/Clash of Minds: Business Edition.jpg',
				posterLowRes: '/events/Clash of Minds: Business Edition-lowres.jpg',
				date: '20th March 2021'
			},
			{
				name: 'Trade Trivia Tournament - Paper Trading',
				poster: '/events/Trade Trivia Tournament - Paper Trading.jpg',
				posterLowRes: '/events/Trade Trivia Tournament - Paper Trading-lowres.jpg',
				date: '20th March 2021'
			},
			{
				name: 'Market Mingle',
				poster: '/events/Market Mingle.jpg',
				posterLowRes: '/events/Market Mingle-lowres.jpg',
				date: '20th March 2021'
			},
			{
				name: 'BizQuiz Bonanza',
				poster: '/events/BizQuiz Bonanza.jpg',
				posterLowRes: '/events/BizQuiz Bonanza-lowres.jpg',
				date: '20th March 2021'
			}
		],
		[
			{
				name: '1-min Speech',
				poster: 'images/event/event1.jpg',
				posterLowRes: 'images/event/event1.jpg',
				date: '20th March 2021'
			},
			{
				name: '1-Min Games',
				poster: 'images/event/event1.jpg',
				posterLowRes: 'images/event/event1.jpg',
				date: '20th March 2021'
			},
			{
				name: 'Biz Hunt',
				posterLowRes: 'images/event/event1.jpg',
				poster: 'images/event/event1.jpg',
				date: '20th March 2021'
			},
			{
				name: 'PublicityPulse: The PR Event',
				poster: 'images/event/event1.jpg',
				posterLowRes: 'images/event/event1.jpg',
				date: '20th March 2021'
			},
			{
				name: 'Design Dual(logo/ tagline/ brand ad)',
				poster: 'images/event/event1.jpg',
				posterLowRes: 'images/event/event1.jpg',
				date: '20th March 2021'
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
											<div class="single-event">
												<img class="img-responsive" src={event.poster} alt={event.name} />
												<h4>{event.name}</h4>
												<p>{event.date}</p>
											</div>
										</div>
									{/each}
								</div>
							</div>
						{/each}
					</div>
				</div>
			</div>
			<div class="guitar">
				<img class="img-responsive" src="images/guitar.png" alt="guitar" />
			</div>
		</div>
	</div>
</section>
