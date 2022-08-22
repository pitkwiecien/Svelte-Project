<script>
    import FixedBar from "../components/FixedBar.svelte";
    import Image from "../components/Image.svelte";
    import Link from "../components/Link.svelte";
    import Button from "../components/Button.svelte";
</script>
<FixedBar heightPercent=10 bgColor="transparent" fontSize=2 bold={true} generateSafeArea={true}>
    <div slot="left" class="rels">
        <Link href="/">
            <Image src="/images/lightbulb.png" alt="logo" scaling=0.02 marginRight=15/>
            <Image src="/images/text.png" alt="company name" scaling = 0.07 marginRight=20/>
        </Link>
        <Link href="/about">O nas</Link>
        <Link href="about:blank">Bezpieczeństwo</Link>
        <Link href="about:blank">Wsparcie</Link>
    </div>
    <div slot="right" class="rels">
        <Button style="secondary">Zaloguj się</Button>
    </div>
</FixedBar>

<style>
    .rels {
            display: flex;
            align-items: center;
        }
</style>