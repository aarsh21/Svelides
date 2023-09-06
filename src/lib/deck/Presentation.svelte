<script lang="ts">
	import Slide from './Slide.svelte';
	import Markdown from './Markdown.svelte';
	import Code from './Code.svelte';
	import Notes from './Notes.svelte';
</script>

<Slide>Horizantal Slide</Slide>

<Slide>
	<Slide>Vertical Slide 1</Slide>
	<Slide>Vertical Slide 2</Slide>
</Slide>

<Slide animate>
	<ul>
		<li>Svelte</li>
		<li>React</li>
		<li>Solid</li>
		<li>Vue</li>
	</ul>
</Slide>

<Slide animate>
	<ul>
		<li>Svelte ❤️</li>
		<li>React</li>
		<li>Solid</li>
		<li>Vue</li>
	</ul>
</Slide>

<Slide animate>
	<Code id="code" lines>
		{`
			function love() {}
	 `}
	</Code>
</Slide>

<Slide animate>
	<Code id="code" lines="2|1-3">
		{`
			function love() {
				console.log('Svelte')
			}
	 `}
	</Code>
</Slide>
<Slide>
	<Markdown>
		{`
            ## Markdown ❤️
            You can use **HTML** or **Markdown** for slides.
        `}
	</Markdown>

	<Notes>
		<b>Avoid eye contact.</b>
	</Notes>
</Slide>
<Slide>
	<Markdown name="example.md" external />
</Slide>
