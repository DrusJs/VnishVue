<template>
    <header class="header">
        <div class="container">
            <div class="header-inner">
                <img src="../assets/img/logo.svg" alt="Logo" class="logo">
                <div class="header-navigation">
                    <nav class="navigation">
                        <ul class="navigation-list">
                            <li class="navigation-list__item"><a href="#firmware">Firmware</a></li>
                            <li class="navigation-list__item"><a href="#advantages">Advantages</a></li>
                            <li class="navigation-list__item"><a href="#about-us">About</a></li>
                            <li class="navigation-list__item"><a href="#faq">FAQ</a></li>
                        </ul>
                    </nav>
                    <ul class="social-media">
                        <li class="social-media__item"><a href="#"><img src="../assets/img/telegram-mono.svg" alt="telegram"></a></li>
                        <li class="social-media__item"><a href="#"><img src="../assets/img/reddit-mono.svg" alt="reddit"></a></li>
                        <li class="social-media__item"><a href="#"><img src="../assets/img/linkedin-mono.svg" alt="linkedin"></a></li>
                        <li class="social-media__item"><a href="#"><img src="../assets/img/facebook-mono.svg" alt="facebook"></a></li>
                        <li class="social-media__item"><a href="#"><img src="../assets/img/youtube-mono.svg" alt="youtube"></a></li>
                        <li class="social-media__item"><a href="#"><img src="../assets/img/twitter-x-mono.svg" alt="twitter"></a></li>
                    </ul>
                </div>
                <button class="burger-button"></button>
            </div>
        </div>
    </header>
</template>
<script>
export default {
    
}
</script>
<style>
.header {
	border-bottom: 1px solid rgba(108, 118, 132, 0.5);
}

.header-inner {
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding: 12px 0;
	gap: 64px;
}

.header-navigation {
	display: flex;
	align-items: center;
	width: 100%;
	justify-content: space-between;
}
.navigation-list {
	display: flex;
	align-items: center;
	gap: 48px;
	list-style: none;
}
.navigation-list__item a {
	color: var(--color-text-primary);
	text-decoration: none;
	transition: 260ms ease-out;
}

.social-media {
	display: flex;
	align-items: center;
	gap: 12px;
	list-style: none;
}
.social-media_item a {
	color: var(--color-text-primary);
	text-decoration: none;
}
.burger-button {
	display: none;
}
</style>