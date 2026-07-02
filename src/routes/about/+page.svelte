<script lang="ts">
    import { PUBLIC_R2_STATIC } from '$env/static/public';
</script>

<main>
    <div class="text-content">
        <h1>About</h1>
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
    <img src="{PUBLIC_R2_STATIC}/hero.png" alt="hero" />
</main>

<style>
    main {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    img {
        width: 650px;
        margin: 4rem 4rem 2rem 2rem;
    }

    .text-content {
        max-width: 700px;
        margin: 1rem 2rem 2rem 5rem;
    }

    h1 {
        font-size: 12rem;
        line-height: 1;
        margin-bottom: 2rem;
    }
</style>
