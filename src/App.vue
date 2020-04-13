<template>
	<div class="home" role="article">
		<div class="form" role="contentinfo">
			<h1>COVID19 IMPACT ESTIMATOR</h1>
			<form>

				<label for="population">Population</label>
				<input
					id="population"
					for="data-population"
					name="data-population"
					data-population=""
					type="number"
          aria-label="population"
					placeholder="Enter population size"
				/>

				<label for="time-period">Time Period</label>
				<input
					id="time-period"
					for="data-time-to-elapse"
					name="data-time-to-elapse"
					data-time-to-elapse=""
					type="number"
          aria-label="time-period"
					placeholder="Enter time period"
				/>

				<label for="time-period-type">Type of time period</label>
				<select data-period-type name="periodType" id="periodType" aria-label="period-type">
              <option value="days">Days</option>
              <option value="weeks">Weeks</option>
              <option value="months">Months</option>
          </select>

				<label for="reported-cases">Number of Reported Cases</label>
				<input
					id="reported-cases"
					for="data-reported-cases"
					name="data-reported-cases"
					data-reported-cases=""
					type="number"
          aria-label="reported-cases"
					placeholder="Enter number of reported cases"
				/>

				<label for="total-hospital-beds">Total Hospital Beds</label>

				<input
					id="total-hospital-beds"
					for="data-total-hospital-beds"
					name="data-total-hospital-beds"
					data-total-hospital-beds=""
					type="number"
          aria-label="hospital-beds"
					placeholder="Enter number of hospital beds"
				/>

				<button
					for="data-go-estimate"
					name="data-go-estimate"
          aria-label="result"
					data-go-estimate=""
					type="submit"
				>
					Submit
				</button>
			</form>
		</div>
	</div>
</template>

<script>

export default {
  name: 'App',
}
</script>

<style>
.home {
	font-family: helvetica, cursive, Arial, sans-serif;
	width: 100%;
	height: 100%;
	box-sizing: border-box;
	margin: 0;
	padding: 0;
	background-color: #f5f5f5;
	position: absolute;
	top: 0;
	right: 0;
	bottom: 0;
	left: 0;
}
h1 {
	font-style: italic;
	font-size: 1.4em;
	margin-top: 0.5em;
}
.form {
	background-color: white;
	min-height: 75vh;
	width: 30%;
	margin: 1em auto;
	padding: 0.1rem 2rem 0.5rem;
	font-weight: bolder;
	font-size: 1.1em;
}
input,
label,
select {
	display: block;
	min-width: 80%;
	height: 2em;
	font-size: 1em;
}
select {
	margin-bottom: 1em;
}
input {
	margin-bottom: 1em;
	border: solid black 1px;
	border-radius: 1px;
	font-size: 1em;
}
button {
	border-radius: 0.5em;
	width: 50%;
	height: 2em;
	font-size: 1em;
	font-weight: bolder;
	background-color: grey;
}
</style>
