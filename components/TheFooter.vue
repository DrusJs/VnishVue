<template>
    <footer class="footer">
        <div class="container">
            <div class="footer-inner">
                <div class="logo">
                    <img src="../assets/img/logo-letter.svg" alt="VnishCom">						
                </div>
                <ul class="footer-list">
                    <div class="footer-list__item"><a href="#">facebook</a></div>
                    <div class="footer-list__item"><a href="#">linkedin</a></div>
                    <div class="footer-list__item"><a href="#">youtube</a></div>
                    <div class="footer-list__item"><a href="#">twitter</a></div>
                </ul>
            </div>
        </div>
    </footer>
</template>
<script>
export default {
    
}
</script>
<style>
.footer {
	border-top: 1px solid rgba(108, 118, 132, 0.5);
}

.footer-inner {
	display: flex;
	padding: 18px 0;
	align-items: center;
	justify-content: space-between;
}
.footer-list {
	list-style: none;
	display: flex;
	align-items: center;
	gap: 40px;
}
.footer-list__item a {
	font-size: 14px;
	font-weight: 600;
	line-height: 16px;
	text-decoration: none;
	color: var(--color-text-primary);
	transition: 260ms ease-out;
}
</style>