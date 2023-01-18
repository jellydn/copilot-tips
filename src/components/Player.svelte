<script>
	export let videoId;
	export let title;
	const thumbnail = `https://i.ytimg.com/vi/${videoId}/hqdefault.jpg`;
</script>

<p>{title}</p>

<lite-youtube videoid={videoId} style={`background-image: url(${thumbnail});`}>
	<a href={`https://youtube.com/watch?v=${videoId}`} class="lty-playbtn" {title}>
		<span class="lyt-visually-hidden">Play Video: {title}</span>
	</a>
</lite-youtube>
