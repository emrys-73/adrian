<script>
    import { browser } from '$app/environment';

    const pdfUrl = '/photopack.pdf';
    
    if (browser) {
        window.location.href = pdfUrl;
    }
</script>

<p>Downloading photoshoot rates...</p>
