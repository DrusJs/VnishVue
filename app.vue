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
	margin-bottom: 32px;
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
</style>
