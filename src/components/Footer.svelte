<script>
	import Linkedin from '../lib/Icons/Linkedin.svelte';
	import Twitter from '../lib/Icons/Twitter.svelte';
	import Instagram from '../lib/Icons/Instagram.svelte';
</script>

<footer>
	<div class="footer-wrapper">
		<div class="credit-wrapper">
			<div class="note-title"><p>Sources:</p></div>
			<div class="note-content">
				<p>Topfeeds farm, National Bureau of statistics, PWC, NNPC, CBN</p>
			</div>
			<div class="note-title"><p>Data Visualization & Development by</p></div>
			<div class="note-content">
				<p>Jayeola Gbenga</p>
			</div>
			<div class="note-title"><p>Research & Written by</p></div>
			<div class="note-content"><p>Jayeola Gbenga</p></div>
			<div class="note-title"><p>Edited by</p></div>
			<div class="note-content"><p>Patsy Nwogu & Blessing Olagunjoye</p></div>
		</div>
		<div class="footer-logo">
			<p>Produced by</p>
		</div>
		<div class="socials-wrapper">
			<ul class="links">
				<li class="social-links symbol">
					<a href="https://www.linkedin.com/company/orodata-science-nigeria/"
						><div class="button linkedin">
							<div class="social">
								<Linkedin />
							</div>
						</div></a
					>
				</li>
				<li class="social-links symbol">
					<a href="https://twitter.com/Orodata"
						><div class="button twitter">
							<div class="social">
								<Twitter />
							</div>
						</div></a
					>
				</li>
				<li class="social-links symbol">
					<a href="https://www.instagram.com/orodatascience/"
						><div class="button instagram">
							<div class="social">
								<Instagram />
							</div>
						</div></a
					>
				</li>
			</ul>
		</div>
	</div>
</footer>

<style>
	footer {
		background: #f4f5f3;
		margin-top: 1rem;
		padding-top: 1.5rem;
		padding-bottom: 1.5rem;
	}

	.footer-wrapper {
		width: 98%;
		max-width: 850px;
		margin: 0 auto;
		overflow-x: hidden;
	}

	.note-title p {
		color: #1b1b1b;
		font-weight: bold;
		font-size: 14px;
		margin-top: 1rem;
		margin-bottom: 0;
		line-height: 1;
	}

	.note-content p {
		color: #747474;
		font-size: 12px;
		margin-bottom: 0;
		margin-top: 0;
	}

	.footer-logo {
		text-align: center;
	}

	.footer-logo p {
		color: #747474;
		font-size: 12px;
		margin-bottom: 0;
	}

	.socials-wrapper {
		text-align: center;
	}

	ul.links {
		display: block;
		padding: 0;
		margin: 0;
		list-style-type: disc;
	}

	.social-links {
		list-style: none;
		display: inline-block;
		vertical-align: middle;
	}

	.social-links a {
		background-color: transparent;
		text-decoration: none;
		color: currentColor;
		text-underline-position: from-front;
	}

	.button.linkedin {
		background: #0072b1;
	}

	.button.twitter {
		background: #000000;
	}

	.button.instagram {
		background: #cd486b;
	}

	.social {
		width: 40px;
		height: 40px;
		display: flex;
		justify-content: center;
		align-items: center;
		color: inherit;
	}
</style>
