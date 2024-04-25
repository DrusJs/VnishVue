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
                <button class="burger-button">
                    <div class="burger-button__open">Menu</div>
                    <div class="burger-button__close">Close</div>
                </button>
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
    padding: 5px 11px;
    align-items: center;
    border: 1px solid #ABB1B9;
    color: #ABB1B9;
	font-family: "Roboto Flex", sans-serif;
    font-size: 14px;
    font-weight: 700;
    border-radius: 30px;
    background-color: transparent;
}
.burger-button__open {
    display: flex;
    align-items: center;
    gap: 6px;
}
.burger-button__open::before {
    content: '';
    display: block;
    width: 17px;
    min-width: 17px;
    height: 17px;
    background-repeat: no-repeat;
    background-position: center center;
    background-image: url("data:image/svg+xml,%3Csvg width='18' height='18' viewBox='0 0 18 18' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M2.69522 6.30432H15.3146C15.5005 6.30432 15.6789 6.23045 15.8103 6.09897C15.9418 5.9675 16.0157 5.78918 16.0157 5.60324C16.0157 5.4173 15.9418 5.23898 15.8103 5.1075C15.6789 4.97602 15.5005 4.90216 15.3146 4.90216H2.69522C2.50928 4.90216 2.33096 4.97602 2.19948 5.1075C2.068 5.23898 1.99414 5.4173 1.99414 5.60324C1.99414 5.78918 2.068 5.9675 2.19948 6.09897C2.33096 6.23045 2.50928 6.30432 2.69522 6.30432V6.30432ZM15.3146 11.9129H2.69522C2.50928 11.9129 2.33096 11.9868 2.19948 12.1183C2.068 12.2498 1.99414 12.4281 1.99414 12.614C1.99414 12.8 2.068 12.9783 2.19948 13.1097C2.33096 13.2412 2.50928 13.3151 2.69522 13.3151H15.3146C15.5005 13.3151 15.6789 13.2412 15.8103 13.1097C15.9418 12.9783 16.0157 12.8 16.0157 12.614C16.0157 12.4281 15.9418 12.2498 15.8103 12.1183C15.6789 11.9868 15.5005 11.9129 15.3146 11.9129ZM15.3146 8.40755H2.69522C2.50928 8.40755 2.33096 8.48141 2.19948 8.61289C2.068 8.74437 1.99414 8.92269 1.99414 9.10863C1.99414 9.29456 2.068 9.47288 2.19948 9.60436C2.33096 9.73584 2.50928 9.8097 2.69522 9.8097H15.3146C15.5005 9.8097 15.6789 9.73584 15.8103 9.60436C15.9418 9.47288 16.0157 9.29456 16.0157 9.10863C16.0157 8.92269 15.9418 8.74437 15.8103 8.61289C15.6789 8.48141 15.5005 8.40755 15.3146 8.40755Z' fill='%23ABB1B9'/%3E%3C/svg%3E");
}
.burger-button__close {
    display: none;
    align-items: center;
    gap: 6px;
}
.burger-button__close::before {
    content: '';
    display: block;
    width: 17px;
    min-width: 17px;
    height: 17px;
    background-repeat: no-repeat;
    background-position: center center;
    background-image: url("data:image/svg+xml,%3Csvg width='18' height='18' viewBox='0 0 18 18' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M9.99378 9.10862L14.4106 4.69884C14.5426 4.56683 14.6168 4.38778 14.6168 4.20108C14.6168 4.01438 14.5426 3.83533 14.4106 3.70331C14.2786 3.5713 14.0995 3.49713 13.9128 3.49713C13.7261 3.49713 13.5471 3.5713 13.415 3.70331L9.00526 8.1201L4.59549 3.70331C4.46347 3.5713 4.28442 3.49713 4.09772 3.49713C3.91102 3.49713 3.73197 3.5713 3.59996 3.70331C3.46794 3.83533 3.39377 4.01438 3.39377 4.20108C3.39377 4.38778 3.46794 4.56683 3.59996 4.69884L8.01674 9.10862L3.59996 13.5184C3.53424 13.5836 3.48209 13.6611 3.4465 13.7465C3.4109 13.832 3.39258 13.9236 3.39258 14.0162C3.39258 14.1087 3.4109 14.2003 3.4465 14.2858C3.48209 14.3712 3.53424 14.4488 3.59996 14.5139C3.66513 14.5796 3.74267 14.6318 3.8281 14.6674C3.91354 14.703 4.00517 14.7213 4.09772 14.7213C4.19027 14.7213 4.28191 14.703 4.36734 14.6674C4.45277 14.6318 4.53031 14.5796 4.59549 14.5139L9.00526 10.0971L13.415 14.5139C13.4802 14.5796 13.5578 14.6318 13.6432 14.6674C13.7286 14.703 13.8203 14.7213 13.9128 14.7213C14.0054 14.7213 14.097 14.703 14.1824 14.6674C14.2679 14.6318 14.3454 14.5796 14.4106 14.5139C14.4763 14.4488 14.5284 14.3712 14.564 14.2858C14.5996 14.2003 14.6179 14.1087 14.6179 14.0162C14.6179 13.9236 14.5996 13.832 14.564 13.7465C14.5284 13.6611 14.4763 13.5836 14.4106 13.5184L9.99378 9.10862Z' fill='%23ABB1B9'/%3E%3C/svg%3E%0A");
}
.burger-button.active .burger-button__open {
    display: none;
}
.burger-button.active .burger-button__close {
    display: flex;
}
</style>