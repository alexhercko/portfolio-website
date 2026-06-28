<script lang="ts">
    import { PUBLIC_R2_STATIC } from '$env/static/public';
</script>

<main>
    <h1>Alex Herčko</h1>
    <div class="hero">
        <img src="{PUBLIC_R2_STATIC}/hero.png" alt="hero" />
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt erat id felis
            semper, sed semper orci pulvinar. Vivamus arcu nibh, dignissim at scelerisque sed,
            eleifend et neque. In ligula ex, vulputate sed magna in, porttitor interdum ligula.
            Mauris congue auctor augue, eu placerat nulla. Vestibulum malesuada et massa a bibendum.
            Ut sit amet ligula quis nibh scelerisque lacinia a eu elit. Fusce in est ut enim tempus
            hendrerit. Nullam tempor magna sed velit hendrerit, et vehicula nibh fringilla.
            Pellentesque nec dui nec justo pellentesque hendrerit vitae sed orci. In aliquam quam
            purus, vitae molestie felis imperdiet sit amet. Nam.
        </p>
    </div>
    <p>Visit <a href="https://github.com/alexhercko">my GitHub page</a>.</p>
</main>

<style>
    main {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    h1 {
        font-size: 12rem;
        margin: 2rem;
    }

    .hero {
        max-width: 1200px;
        display: flex;
        flex-direction: row;
    }

    .hero img {
        width: 500px;
        margin: 2rem 4rem 2rem 2rem;
    }

    .hero p {
        margin: 2rem;
    }
</style>
