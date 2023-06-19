---
label: Chris's Suggestion 
icon: star
order: -997
---
<html>
<head>
	<title>Toggle Dark and Light Mode</title>
	<style>
		html {
			transition: background-color 0.5s ease;
			color: black;
		}
		html.dark {
			background-color: #121212;
			color: white;
		}
		.modeImage {
			width: 100px;
			height: 100px;
			background-image: url('/static/sample-text-black.png');
			background-size: cover;
			background-position: center;
		}
		html.dark .modeImage {
			background-image: url('/static/sample-text-white.png');
		}
	</style>
	<script>
		function toggleDarkLightMode() {
			var html = document.documentElement;
			html.classList.toggle("dark");
		}
	</script>
</head>
<body>
	<div class="modeImage"></div>
</body>
</html>

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.