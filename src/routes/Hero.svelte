<script>
	let eventRegistrationText = 'Event Registration';
	let partiticapteEventSubText = 'Participate in the event';
</script>

<section id="home">
	<div id="main-slider" class="carousel slide" data-ride="carousel">
		<ol class="carousel-indicators">
			<li data-target="#main-slider" data-slide-to="0" class="active"></li>
			<li data-target="#main-slider" data-slide-to="1"></li>
			<li data-target="#main-slider" data-slide-to="2"></li>
		</ol>
		<div class="carousel-inner">
			<div class="item active">
				<div class="layer"></div>
				<img class="img-responsive" src="pexels-helena-lopes-1015568.jpg" alt="slider" />
				<!-- <img class="img-responsive" src="images/slider/bg1.jpg" alt="slider" /> -->
				<div class="carousel-caption">
					<h2>{eventRegistrationText}</h2>
					<h4>{partiticapteEventSubText}</h4>
					<a href="https://linktr.ee/mitipsum"
						>GRAB YOUR TICKETS <i class="fa fa-angle-right"></i></a
					>
				</div>
			</div>
			<div class="item">
				<div class="layer"></div>
				<img class="img-responsive" src="pexels-shvets-production-7561874.jpg" alt="slider" />
				<div class="carousel-caption">
					<h2>{eventRegistrationText}</h2>
					<h4>{partiticapteEventSubText}</h4>
					<a href="https://linktr.ee/mitipsum"
						>GRAB YOUR TICKETS <i class="fa fa-angle-right"></i></a
					>
				</div>
			</div>
			<div class="item">
				<div class="layer"></div>
				<img class="img-responsive" src="pexels-stiven-rivera-17558082.jpg" alt="slider" />
				<div class="carousel-caption">
					<h2>{eventRegistrationText}</h2>
					<h4>{partiticapteEventSubText}</h4>
					<a href="https://linktr.ee/mitipsum"
						>GRAB YOUR TICKETS <i class="fa fa-angle-right"></i></a
					>
				</div>
			</div>
		</div>
	</div>
</section>

<style>
	.item {
		position: relative;
	}
	.item .layer {
		position: absolute;
		inset: 0;
		background-color: rgba(0, 0, 0, 0.6);
	}
</style>
