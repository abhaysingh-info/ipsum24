<script>
	let days = 0;
	let hours = 0;
	let minutes = 0;
	let seconds = 0;

	const date = new Date('2024-02-02T10:00:00');

	setInterval(() => {
		const currentTime = new Date();
		const diff = date.getTime() - currentTime.getTime();
		days = Math.floor(diff / (1000 * 60 * 60 * 24));
		hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
		minutes = Math.floor((diff / 1000 / 60) % 60);
		seconds = Math.floor((diff / 1000) % 60);
	}, 1000);
</script>

<section id="explore">
	<div class="container">
		<div class="row">
			<div class="watch">
				<img class="img-responsive" src="images/watch.png" alt="" />
			</div>
			<div class="col-md-4 col-md-offset-2 col-sm-5">
				<h2>Event Starts In</h2>
			</div>
			<div class="col-sm-7 col-md-6">
				<ul id="countdown">
					<li>
						<span class="days time-font" id="Days">{days}</span>
						<p>days</p>
					</li>
					<li>
						<span class="hours time-font" id="Hours">{hours}</span>
						<p class="">hours</p>
					</li>
					<li>
						<span class="minutes time-font" id="Minutes">{minutes}</span>
						<p class="">minutes</p>
					</li>
					<li>
						<span class="seconds time-font" id="Seconds">{seconds}</span>
						<p class="">seconds</p>
					</li>
				</ul>
			</div>
		</div>
		<div class="cart">
			<a href="#"
				><i class="fa fa-shopping-cart"></i>
				<span>Purchase Tickets</span></a
			>
		</div>
	</div>
	<!-- </section> -->
</section>
