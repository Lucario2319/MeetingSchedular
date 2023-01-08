<script>
    import FeedbackItem from "./FeedbackItem.svelte";
    export let feedback = [];
</script>

<h2>Feedback List</h2>
{#each feedback as fb (fb.id)}
    <FeedbackItem item={fb} />
{/each}