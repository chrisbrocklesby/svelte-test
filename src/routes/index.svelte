<script>
  import TestComponent from "../components/test.svelte";
  const test = `This is a constant {a bit like this} just testing it... It works !`;
  const items = ['one', 'two', 'three'];
</script>


<h1>Welcome to the home page</h1>
<p>{test}</p>
<TestComponent />
<p><a href="/about">About</a></p>
<ul>
  <li>Array Loop of items test</li>
  {#each items as item}
    <li>{item}</li>
  {/each}
</ul>

<p>Think I am starting to love Svelte ! - Wow</p>