<script>
import Picture from '../Picture.svelte';
const headshot = 'headshot.jpg';
const eyeball = 'eyeball.png';

</script>

<div class="pictures">
    <Picture>
        <img src={headshot} alt="James Freeman headshot" />
    </Picture>

    <Picture>
        <p>
            <a href="https://blog.apollo350.com/posts/easy-ci-cd-with-github-actions">Easy CI/CD with Github Actions</a>
        </p>
    </Picture>

    <Picture>
        <h1>James Freeman</h1>
    </Picture>

    <Picture>
        <p>
            <a href="https://blog.apollo350.com/posts/video-calls-in-the-time-of-covid">Video Calls in the Time of Covid</a>
        </p>
    </Picture>

    <Picture>
        <iframe src="https://jammaloo.com/faces/"></iframe>
    </Picture>

    <Picture>
        <a href="https://jammaloo.com/random/EyeSeeYou/dist/">
            <img src={eyeball} alt="A colourful eyeball" />
        </a>
    </Picture>
</div>

<style>
    iframe {
        border: none;
    }
    .pictures {
    }
</style>
