<template>
  <div class="wrapper">
      <TheHeader />
      <TheMain />
      <TheFooter />
  </div>
</template>
<script>
export default {
  
}
</script>
<style>
  :root {
	--color-dark-bg: #0E1011;
	--color-white: #FFFFFF;
	--color-text-primary: #DCDFE5;
	--color-text-secondary: #6C7684;
	--color-primary: #D19A66;
	--color-stroke: #373D48;
	--linear-gradient-grid: linear-gradient(to bottom, rgba(255, 255, 255, 0.06), rgba(255, 255, 255, 0.03))
}

* {
	margin: 0;
	padding: 0;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}

*:before, *:after {
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}

html {
	scroll-behavior: smooth;
}

body {
	background-color: var(--color-dark-bg);
	color: var(--color-white);
	font-family: "Roboto Flex", sans-serif;
}

h1.main-title {
	font-size: 88px;
	font-weight: 500;
	line-height: 80px;
	text-align: center;
	max-width: 1000px;
	margin: 0 auto 32px;
}

h2.title {
	font-size: 64px;
	font-weight: 500;
	line-height: 64px;
	letter-spacing: -1.6px;
	text-align: center;
	margin-bottom: 24px;
}

.title_large {
	font-size: 36px;
	font-weight: 500;
	line-height: 40px;
}
.title_medium {
	font-size: 24px;
	font-weight: 500;
	line-height: 30px;
}
.text_large {
	font-size: 24px;
	font-weight: 400;
	line-height: 30px;
}
.text_medium {
	font-size: 16px;
	font-weight: 400;
	line-height: 22px;
}
.action_medium {
	font-size: 14px;
	font-weight: 600;
	line-height: 22px;
	color: #ABB1B9;
}
.accent {
	font-style: italic;
	font-size: 64px;
	font-weight: 400;
	line-height: 64px;
	letter-spacing: -1px;
	padding-right: 4px;
}
.text_center {
	text-align: center;
}
.color_primary {
	color: var(--color-primary);
}
.color_white {
	color: var(--color-white);
}
.color_text {
	color: var(--color-text-primary);
}
a.text_link {
	color: var(--color-primary);
	text-decoration: underline;
}

.button {
	font-family: "Roboto Flex", sans-serif;
	font-size: 16px;
	font-weight: 600;
	line-height: 20px;
	color: var(--color-dark-bg);
	background-color: var(--color-primary);
	border: 1px solid transparent;
	border-radius: 100px;
	height: 55px;
	display: flex;
	align-items: center;
	white-space: nowrap;
	justify-content: center;
	gap: 8px;
	padding: 12px 24px;
	transition: 260ms ease-out;
	cursor: pointer;
}
.button svg {
	min-width: 25px;
}
.button.blue-button {
	background-color: transparent;
	color: #83CFF8;
	border: 1px solid #83CFF8;
}
.button.stroke {
	color: var(--color-white);
	border: 1px solid var(--color-white);
	background-color: rgba(255, 255, 255, 0.03);
}
.wrapper {
	display: flex;
	flex-direction: column;
	min-height: 100vh;
	background-image: url(../img/background.png);
	position: top center;
	background-repeat: no-repeat;
	background-size: cover;
}

.container {
	width: 100%;
	max-width: 1280px;
	padding: 0 64px;
	margin: 0 auto;
}

@media (max-width: 1050px) {
	.advantages-grid {
		grid-template-columns: 1fr;
		grid-template-rows: auto;
	}
	.advantages-grid__item_long {
		grid-column: 1;
	}
	.about-flex {
		flex-wrap: wrap;
	}
	.firmware-head {
		flex-wrap: wrap;
		justify-content: flex-start;
	}	
	.firmware-image img {
		width: 100%;
		max-width: 280px;
	}
}

@media (max-width: 876px) {
	.container {
		padding: 0 26px;
	}
	.main-actions {
		flex-direction: column;
	}
	.advantages-grid.height-auto {
		grid-template-columns: 1fr;
	}
	.header-navigation {
		position: fixed;
		top: 100%;
	}
	.burger-button {
		display: flex;
	}
	.main-section {
		padding: 80px 0 42px;
	}
	.bg-section {
		padding-top: 76px;
	}
	.firmware-head {
		flex-direction: column;
	}
	.select-label {
		font-size: 24px;
	}
	.select-primary, .select-value {
		width: 100%;
	}
	.select-head {
		display: grid;
		grid-template-columns: 0.6fr 1.3fr;
	}
	.advantages-grid__item-img img {
		width: 100%;
	}
	.firmware-image {
		display: none;
	}
	.firmware-inner {
		padding: 32px 24px;
	}
	.firmware-info {
		text-align: center;
	}
	.firmware-flex {
		justify-content: center;
		text-align: center;
	}
	.firmware-item .button, .firmware-item {
		width: 100%;
		max-width: none;
	}
	h1.main-title {
		font-size: 50px;
		line-height: 48px;
	}

	h2.title {
		font-size: 40px;
		line-height: 40px;
	}
	.accent {
		font-size: 32px;
		line-height: 40px;
	}
	.about-flex .accent {
		font-size: 64px;
		line-height: 64px;
	}
}
@media (max-width: 546px) {
	.container {
		padding: 0 16px;
	}
	.footer-inner {
		flex-direction: column;
		justify-content: center;
		gap: 26px;
	}
}
</style>
