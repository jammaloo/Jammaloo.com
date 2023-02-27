<script>
import Picture from '../Picture.svelte';
let headshot = 'headshot.jpg';

</script>
<h1>James Freeman</h1>
<Picture>
    <img src={headshot} alt="James Freeman headshot" />
</Picture>
<Picture>
    <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
</Picture>
