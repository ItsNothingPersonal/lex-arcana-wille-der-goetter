<script>
	import '../../app.css';
</script>

<div class="flex flex-col">
	<div class="flex flex-row w-full justify-center">
		<div
			class="prose prose-stone min-w-min font-serif prose-p:leading-relaxed 
			prose-p:text-justify lg:prose-xl prose-figcaption:text-sm 
			prose-figcaption:text-stone-900 prose-blockquote:text-stone-900 
			prose-blockquote:leading-relaxed prose-blockquote:text-justify prose-ul:text-left 
			prose-ol:text-left prose-li:text-justify px-4"
		>
			<slot />
		</div>
	</div>
</div>
