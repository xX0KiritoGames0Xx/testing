# testing
<button onclick="sharePage()">Share</button>

<script>
async function sharePage() {
  if (navigator.share) {
    await navigator.share({
      title: "My Site",
      text: "Check this out!",
      url: window.location.href
    });
  }
}
</script>
