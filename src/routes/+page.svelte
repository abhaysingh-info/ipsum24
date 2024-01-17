<script>
	import Hero from './Hero.svelte';

	import Countdown from './Countdown.svelte';

	import EventsCarousel from './events/EventsCarousel.svelte';

	import Footer from './Footer.svelte';

	import Contact from './Contact.svelte';

	import Sponsors from './Sponsors.svelte';

	import About from './About.svelte';

	import Navbar from './Navbar.svelte';
</script>

<svelte:head>
	<link href="css/bootstrap.min.css" rel="stylesheet" />
	<link href="css/font-awesome.min.css" rel="stylesheet" />
	<link href="css/main.css" rel="stylesheet" />
	<link href="css/animate.css" rel="stylesheet" />
	<link href="css/responsive.css" rel="stylesheet" />

	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta name="description" content="" />
	<meta name="author" content="" />
	<title>IPSUM 2K24</title>

	<link rel="shortcut icon" href="images/ico/favicon.ico" />
	<link
		rel="apple-touch-icon-precomposed"
		sizes="144x144"
		href="images/ico/apple-touch-icon-144-precomposed.png"
	/>
	<link
		rel="apple-touch-icon-precomposed"
		sizes="114x114"
		href="images/ico/apple-touch-icon-114-precomposed.png"
	/>
	<link
		rel="apple-touch-icon-precomposed"
		sizes="72x72"
		href="images/ico/apple-touch-icon-72-precomposed.png"
	/>
	<link rel="apple-touch-icon-precomposed" href="images/ico/apple-touch-icon-57-precomposed.png" />

	<script type="text/javascript" src="js/jquery.js" defer></script>
	<script type="text/javascript" src="js/bootstrap.min.js" defer></script>
	<script
		type="text/javascript"
		src="http://maps.google.com/maps/api/js?sensor=true"
		defer
	></script>
	<script type="text/javascript" src="js/gmaps.js" defer></script>
	<script type="text/javascript" src="js/smoothscroll.js" defer></script>
	<script type="text/javascript" src="js/jquery.parallax.js" defer></script>
	<script type="text/javascript" src="js/coundown-timer.js" defer>
	</script>
	<script type="text/javascript" src="js/jquery.scrollTo.js" defer></script>
	<script type="text/javascript" src="js/jquery.nav.js" defer></script>
	<script type="text/javascript" src="js/main.js" defer></script>
</svelte:head>

<Navbar></Navbar>
<Hero></Hero>
<Countdown></Countdown>
<EventsCarousel></EventsCarousel>
<About></About>
<!-- <Sponsors></Sponsors> -->
<Contact></Contact>
<Footer></Footer>
