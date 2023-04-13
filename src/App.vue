<template>
	<div class="container">
		<div class="card-container">
			<div class="cards left">
				<p>Your Result</p>
				<div class="result">
					<span class="score">76</span>
					<span class="percentage">of 100</span>
				</div>
				<p>Great</p>
				<p>
					You scored higher than 65% of the people who have taken these tests
				</p>
			</div>
			<div class="cards right">
				<h3>Summary</h3>
				<div class="summary-container">
					<div class="summary-item">
						<span class="summary-subject">
							<span class="subject-icon"
								><img src="./components/icons/bolt.svg" alt=""
							/></span>
							Reaction</span
						>
						<span class="summary-score">
							<span class="summary-score-percentage">80</span> / 100
						</span>
					</div>
					<div class="summary-item">
						<span class="summary-subject">
							<span class="subject-icon"
								><img src="./components/icons/brain.svg" alt="" /></span
							>Memory
						</span>
						<span class="summary-score">
							<span class="summary-score-percentage">92</span> / 100
						</span>
					</div>
					<div class="summary-item">
						<span class="summary-subject">
							<span class="subject-icon"
								><img src="./components/icons/verbal.svg" alt="" /></span
							>Verbal</span
						>
						<span class="summary-score">
							<span class="summary-score-percentage">61</span> / 100
						</span>
					</div>
					<div class="summary-item">
						<span class="summary-subject">
							<span class="subject-icon"
								><img src="./components/icons/visual.svg" alt="" /></span
							>Visual</span
						>
						<span class="summary-score">
							<span class="summary-score-percentage">72</span> / 100
						</span>
					</div>
				</div>
				<button>Continue</button>
			</div>
		</div>
	</div>
</template>

<script setup></script>

<style scoped>
	.container {
		padding: 20%;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.card-container {
		display: flex;
		box-shadow: 28px 38px 32px -33px var(--neutral-light-lavender);
		border-radius: 3rem;
	}

	.card-container > .cards {
		width: 24rem;
	}

	.card-container > .left {
		background: linear-gradient(
			var(--light-slate-blue),
			var(--light-royal-blue)
		);
		border-radius: 3rem;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.card-container > .left > p:first-child {
		color: hsl(241, 100%, 89%);
		font-weight: 500;
		font-size: 1.5rem;
		margin: 1rem 0;
	}

	.left > .result {
		background: linear-gradient(var(--violet-blue), var(--persian-blue));
		height: 14rem;
		width: 14rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		border-radius: 50%;
	}

	.score {
		color: var(--neutral-white);
		font-size: 4rem;
		font-weight: 900;
		height: 4rem;
		margin-bottom: 1rem;
	}

	.percentage {
		color: var(--neutral-light-lavender);
	}

	div.cards:nth-child(1) > p:nth-child(3) {
		color: var(--neutral-white);
		font-size: 2rem;
		margin: 1rem 0;
		font-weight: 700;
	}

	div.cards:nth-child(1) > p:nth-child(4) {
		text-align: center;
		height: 7rem;
		padding: 0 16%;
		color: var(--neutral-light-lavender);
	}

	.right {
		padding: 2rem 2rem;
	}

	.right > h3 {
		margin: 1rem 0;
		color: var(--neutral-dark-gray-blue);
		font-size: 1.5rem;
		font-weight: 700;
	}

	.summary-item {
		margin: 0 0 1rem 0;
		padding: 0.5rem 1rem;
		display: flex;
		justify-content: space-between;
		height: 4rem;
		align-items: center;
		border-radius: 0.5rem;
	}

	/*Subject- Reaction */
	.summary-item:nth-child(1) {
		background: hsla(0, 100%, 67%, 0.1);
	}

	.summary-item > span.summary-subject {
		font-weight: 700;
		display: flex;
	}

	div.summary-item:nth-child(1) > span:nth-child(1) {
		color: var(--light-red);
	}

	.subject-icon {
		display: flex;
		margin-right: 0.2rem;
	}

	/*Subject- Memory */
	div.summary-item:nth-child(2) {
		background: hsla(38.8, 100%, 56.1%, 0.1);
	}

	div.summary-item:nth-child(2) > span:nth-child(1) {
		color: var(--orange);
	}

	/*Subject- Verbal */
	div.summary-item:nth-child(3) {
		background: hsla(166, 100%, 37.1%, 0.1);
	}

	div.summary-item:nth-child(3) > span:nth-child(1) {
		color: var(--green-teal);
	}

	/*Subject- Verbal */
	div.summary-item:nth-child(4) {
		background: hsla(233.8, 85.2%, 44.9%, 0.1);
	}

	div.summary-item:nth-child(4) > span:nth-child(1) {
		color: var(--cobalt-blue);
	}

	/**summary score section */
	.summary-score-percentage {
		font-weight: 700;
		color: var(--neutral-dark-gray-blue);
	}

	.summary-score {
		color: var(--neutral-light-lavender);
	}

	/**button */
	div.cards:nth-child(2) > button:nth-child(3) {
		width: 100%;
		height: 3rem;
		border-radius: 2em;
		background: var(--neutral-dark-gray-blue);
		color: var(--neutral-pale-blue);
		font-weight: 700;
		margin-top: 1rem;
	}

	@media only screen and (max-width: 429px) {
		.card-container {
			flex-direction: column;
		}
	}
</style>
