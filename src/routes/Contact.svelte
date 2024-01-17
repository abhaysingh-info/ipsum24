<script>
	const handleSubmit = (event) => {
		event.preventDefault();

		const myForm = event.target;
		const formData = new FormData(myForm);

		fetch('/', {
			method: 'POST',
			headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
			body: new URLSearchParams(formData).toString()
		})
			.then(() => console.log('Form successfully submitted'))
			.catch((error) => alert(error));
	};
</script>

<section id="contact">
	<!-- <div id="map">
				<div id="gmap-wrap">
					<div id="gmap"></div>
				</div>
			</div> -->
	<!--/#map-->
	<div class="contact-section">
		<div class="ear-piece">
			<img class="img-responsive" src="images/ear-piece.png" alt="" />
		</div>
		<div class="container">
			<div class="row">
				<div class="col-sm-3 col-sm-offset-4">
					<div class="contact-text">
						<h3>Contact</h3>
						<address>
							E-mail: promo@party.com<br />
							Phone: +1 (123) 456 7890<br />
							Fax: +1 (123) 456 7891
						</address>
					</div>
					<div class="contact-address">
						<h3>Contact</h3>
						<address>
							Unit C2, St.Vincent's Trading Est.,<br />
							Feeder Road,<br />
							Bristol, BS2 0UY<br />
							United Kingdom
						</address>
					</div>
				</div>
				<div class="col-sm-5">
					<div id="contact-section">
						<h3>Send a message</h3>
						<div class="status alert alert-success" style="display: none"></div>
						<form
							id="main-contact-form"
							class="contact-form"
							name="contact-form"
							netlify
							on:submit={handleSubmit}
						>
							<!-- method="post" -->
							<!-- action="sendemail.php" -->
							<div class="form-group">
								<input type="text" name="name" class="form-control" placeholder="Name" required />
							</div>
							<div class="form-group">
								<input
									type="email"
									name="email"
									class="form-control"
									placeholder="Email ID"
									required
								/>
							</div>
							<div class="form-group">
								<textarea
									name="message"
									id="message"
									class="form-control"
									rows="4"
									placeholder="Enter your message"
									required
								></textarea>
							</div>
							<div class="form-group">
								<button type="submit" class="btn btn-primary pull-right"> Send </button>
							</div>
						</form>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
