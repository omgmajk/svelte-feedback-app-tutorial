<script>
	import FeedbackForm from './components/FeedbackForm.svelte';
	import FeedbackList from './components/FeedbackList.svelte';
	import FeedbackStats from './components/FeedbackStats.svelte';

</script>

<main class="container"> <!-- Can have class directly on the <main> tag -->
	<FeedbackForm />
	<FeedbackStats />
	<FeedbackList /> <!-- feedback={feedback} is the same as {feedback}-->
</main>

<style>

</style>