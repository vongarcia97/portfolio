<script>
  import { onMount } from 'svelte';
  import '../app.css';
  import PageTransition from '$lib/PageTransition.svelte';

  export let data;

  let intro = false;

  onMount(() => {
    intro = true;
  })
</script>


<PageTransition key={data.url} duration={600}>
  {#if !intro}
  <h1>LOADING.....</h1>
  {:else}
  <slot/>
  <div class="flex justify-center mt-36 pb-32 px-2">
    <p class="text-slate-100 dark:text-slate-100 text-xs md:text-lg md:px-4">
      Software Engineer
    </p>
    <p class="text-slate-300 dark:text-slate-300 text-xs md:text-lg px-4">
      |
    </p>
    <p class="text-slate-100 dark:text-slate-100 text-xs md:text-lg md:px-4">
      Von Garcia
    </p>
    <p class="text-slate-300 dark:text-slate-300 text-xs md:text-lg px-4">
      |
    </p>
    <p class="text-slate-100 dark:text-slate-100 text-xs md:text-lg md:px-4">
      New York, NY
    </p>
  </div>
  {/if}
</PageTransition>
  
<div class="btm-nav">
  <a href="/">
    <button>
      <svg xmlns="http://www.w3.org/2000/svg" height="48" width="48"><path d="M11.3 34.7q3.1-2.1 6.15-3.225Q20.5 30.35 24 30.35q3.55 0 6.65 1.175 3.1 1.175 6.1 3.175 2.1-2.75 2.95-5.275.85-2.525.85-5.425 0-7-4.775-11.775T24 7.45q-7 0-11.775 4.775T7.45 24q0 2.9.85 5.4.85 2.5 3 5.3ZM24 25.85q-3.05 0-5.1-2.05t-2.05-5.1q0-3 2.05-5.075T24 11.55q3.05 0 5.1 2.075t2.05 5.125q0 3-2.05 5.05T24 25.85Zm0 19.4q-4.35 0-8.225-1.675T9 39q-2.9-2.9-4.575-6.775Q2.75 28.35 2.75 24t1.675-8.225Q6.1 11.9 9 9q2.9-2.9 6.775-4.6Q19.65 2.7 24 2.7t8.225 1.7Q36.1 6.1 39 9q2.9 2.9 4.6 6.775Q45.3 19.65 45.3 24t-1.7 8.225Q41.9 36.1 39 39q-2.9 2.9-6.775 4.575Q28.35 45.25 24 45.25Zm0-4.7q2.6 0 4.975-.7 2.375-.7 4.925-2.55-2.6-1.75-4.95-2.575Q26.6 33.9 24 33.9t-4.925.825q-2.325.825-4.925 2.575 2.55 1.85 4.9 2.55 2.35.7 4.95.7Zm0-18.3q1.55 0 2.55-.975 1-.975 1-2.575 0-1.55-1-2.55-1-1-2.55-1-1.55 0-2.55 1-1 1-1 2.55 0 1.6 1 2.575 1 .975 2.55.975Zm0-3.55Zm.05 18.55Z"/></svg>
    </button>
  </a>
  <a href="/webapps">
    <button class="active">
      <svg xmlns="http://www.w3.org/2000/svg" height="48" width="48"><path d="M7.45 41.25q-1.95 0-3.325-1.375Q2.75 38.5 2.75 36.55v-25.1q0-1.95 1.375-3.35Q5.5 6.7 7.45 6.7h33.1q1.95 0 3.35 1.4 1.4 1.4 1.4 3.35v25.1q0 1.95-1.4 3.325-1.4 1.375-3.35 1.375Zm0-4.7h33.1v-20.9H7.45v20.9ZM15 33.4l-2.1-2.1 5.15-5.2-5.2-5.2L15 18.8l7.3 7.3Zm9.5.2v-3h11v3Z"/></svg>
    </button>
  </a>
  <a href="/connect">
    <button>
      <svg xmlns="http://www.w3.org/2000/svg" height="48" width="48"><path d="M21.95 35.25H14q-4.7 0-7.975-3.275Q2.75 28.7 2.75 24q0-4.7 3.275-8T14 12.7h7.95v4.75H14q-2.75 0-4.65 1.9-1.9 1.9-1.9 4.65 0 2.75 1.9 4.65 1.9 1.9 4.65 1.9h7.95ZM15.4 25.8v-3.6h17.2v3.6Zm10.65 9.45v-4.7H34q2.75 0 4.65-1.9 1.9-1.9 1.9-4.65 0-2.75-1.9-4.65-1.9-1.9-4.65-1.9h-7.95V12.7H34q4.7 0 8 3.3t3.3 8q0 4.7-3.3 7.975-3.3 3.275-8 3.275Z"/></svg>
    </button>
  </a>
</div>
