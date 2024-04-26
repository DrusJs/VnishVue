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
	--color-page: #21252A;
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

.action_large {
	font-size: 16px;
	font-weight: 600;
	line-height: 20px;
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
.fade {
	opacity: 0;
	transform: translateY(-20px);
	transition: transform 0.6s, opacity 0.6s;
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
.button span.size {
	font-weight: 400;
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
	background-image: url(img/background.png);
	background-position: top center;
	background-repeat: no-repeat;
	background-size: cover;
}
.header {
	position: fixed;
	width: 100%;
	top: 0;
	z-index: 2;
	background-color: #2B2D35;
}
.firmware-section {
	position: relative;
	z-index: 1;
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
	
	.firmware-image img {
		width: 100%;
		max-width: 280px;
	}
	.firmware-head {
		grid-template-columns: 1fr 1fr;
		justify-items: flex-start;
	}
}

@media (max-width: 876px) {
	body:has(.header-navigation.active) {
		overflow: hidden;
	}

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
		top: 73px;
		padding-top: 48px;
		left: auto;
		right: -100%;
		height: calc(100dvh - 100px);
		display: flex;
		flex-direction: column;
		box-shadow: 100px 100px 0 100px #2B2D35;
		background-color: #2B2D35;
		transition: 200ms ease-out;
	}
	.navigation-list {
		flex-direction: column;
		gap: 36px;
	}
	.navigation-list__item a {
		font-size: 24px;
		line-height: 30px;
		font-weight: 500;
	}
	.header-navigation.active {
		right: 0;
	}
	.social-media {
		width: 100%;
		justify-content: center;
		padding-top: 16px;
		border-top: 1px solid var(--color-stroke);
	}
	.burger-button {
		display: flex;
	}
	.main-section {
		padding: 153px 0 42px;
	}
	.bg-section {
		padding-top: 76px;
	}
	.select-wrapper {
		display: grid;
		grid-template-columns: 84px 1fr;
		width: 100%;
	}
	.firmware-head {
		flex-direction: column;
		padding: 18px;
	}
	.select-primary, .select-value {
		width: 100%;
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
	.about-container {
		padding: 46px 18px;
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
	.navigation-list {
		gap: 24px;
	}
	.firmware-head {
		grid-template-columns: 1fr;
	}
}
@media (max-width: 359px) {
	.header-navigation {
		padding-top: 26px;
	}
	.header-navigation {
		height: calc(100dvh - 84px);
	}
	.footer-list {
		gap: 26px;
	}
}
@media (hover: hover) {
    .navigation-list__item a:hover,
	.footer-list__item a:hover {
		color: var(--color-white);
	}
	.social-media__item:hover path {
		fill: var(--color-white);
	}
}
</style>
