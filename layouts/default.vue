<template>
	<div class="container">
		<CThemeProvider>
			<CColorModeProvider>
				<CBox font-family="body" as="main" class="main">
					<CReset />
						<Navbar />
						<Nuxt />
				</CBox>
			</CColorModeProvider>
		</CThemeProvider>
	</div>
</template>
<script>
	import {
		CThemeProvider,
		CColorModeProvider,
		CReset,
		CBox
	} from '@chakra-ui/vue'

	import Navbar from "../components/Navbar.vue"

	export default {
		name: 'App',
		components: {
			CThemeProvider,
			CColorModeProvider,
			CReset,
			CBox,
			Navbar
		}
	}
</script>
<style>
* {
	font-family: "Poppins", sans-serif;
	scroll-behavior: smooth;
}
.main {
	background-image: linear-gradient(147deg, #000000 0%, #04619f 74%);
	color: #f2e5ff;
}
</style>