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

	<!--/#map-->

	<div class="contact-section">
		<div class="ear-piece">
			<img class="img-responsive" src="images/ear-piece.png" alt="" />
		</div>
		<div class="container">
			<div class="row">
				<div class=" col-sm-offset-5">
					<div class="d-flex">
						<div class="contact-text">
							<h3>Faculty Co-ordinator</h3>
							<address>
								Name: Dr. S.S. Patil<br />
								E-mail: sspatil@mitacsc.ac.in<br />
								Phone: +91 8329896244<br />
							</address>
						</div>
						<div class="contact-text">
							<h3>Student Coordinator</h3>
							<address>
								Name: Sania Inamdar<br />
								E-mail: saniainamdar9494@gmail.com<br />
								Phone: +91 8010761591<br />
							</address>
						</div>
						<div class="contact-address">
							<h3>Address</h3>
							<address>
								MIT Arts Commerce and Science College,<br />
								Moshi - Alandi Rd,<br />
								opposite Gajanan Maharaj<br />
								Sansthan, Alandi, Pune,<br />
								Maharashtra 412105
							</address>
						</div>
					</div>
				</div>
				<!-- <div class="col-sm-5">
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
				</div> -->
			</div>
		</div>
	</div>
</section>

<style>
	.contact-section {
		overflow: hidden;
	}

	.d-flex {
		display: flex !important;
	}
</style>
