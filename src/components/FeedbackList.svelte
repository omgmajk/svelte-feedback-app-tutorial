<script>
  //import {onMount, onDestroy} from 'svelte';
  import {FeedbackStore} from '../stores.js';
  import {fade, scale} from 'svelte/transition';
  import FeedbackItem from './FeedbackItem.svelte';
  // let feedback = [];

  // const unsubscribe = FeedbackStore.subscribe((data) => feedback = data);

  // onDestroy(() => {
  //   unsubscribe();
  // });
</script>
<!-- Doing it like $FeedbackStore does all of the above including unsubscribe -->
{#each $FeedbackStore as fb(fb.id)}
  <div in:scale out:fade="{{duration: 500}}">
    <FeedbackItem item={fb} />
  </div>
{/each}