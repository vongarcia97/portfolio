<script>
  import {onMount} from 'svelte';
  import { fade, scale, slide } from 'svelte/transition';
  import { bounceInOut, quintInOut } from 'svelte/easing';

</script>

<div id="bitepay-container" class="flex">
  <div class="relative max-w-5xl mx-auto px-10 pt-20 sm:pt-24 lg:pt-32">
    <h1 in:scale={{  duration: 1000, easing: bounceInOut }} class="text-white font-extrabold text-4xl sm:text-5xl lg:text-6xl tracking-tight text-center"><a href="http://bitepaynyc-env.eba-jjnppubt.us-east-1.elasticbeanstalk.com/" target="_blank" rel="noreferrer" >
      BitePay-NYC
    </a>
    </h1>
    <h1 in:fade={{ delay: 250, duration: 2000, easing: quintInOut }} class="text-slate-400 font-extrabold text-2xl md:text-3xl lg:text-5xl tracking-tight text-center">Only pay for what you bit.</h1>
    <p in:slide={{ delay: 1500, duration: 2000, easing: bounceInOut }} class="mt-6 text-sm md:text-lg text-slate-300 text-center tracking-widest max-w-3xl mx-auto">Frontend: 
      <code class="font-mono font-medium text-lime-500">
        React.js
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        Tailwindcss
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        Webpack
      </code>
    </p>
    <p in:slide={{ delay: 1500, duration: 2000, easing: bounceInOut }} class="mt-6 text-sm md:text-lg text-slate-300 text-center tracking-widest max-w-3xl mx-auto">Backend: 
      <code class="font-mono font-medium text-lime-500">
        Node.js
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        Express.js
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        WebSockets
      </code>
    </p>
    <p in:slide={{ delay: 1500, duration: 2000, easing: bounceInOut }} class="mt-6 text-sm md:text-lg text-slate-300 text-center tracking-widest max-w-3xl mx-auto">Devops:
      <code class="font-mono font-medium text-lime-500">
        Docker
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        AWS EC2
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        ElasticBeanstalk
      </code>
    </p>
  </div>
</div>
<div id="bitepay-container" class="flex">
  <div class="relative max-w-5xl mx-auto px-10 pt-20 sm:pt-24 lg:pt-32">
    <h1 in:scale={{  duration: 1000, easing: bounceInOut }} class="text-white font-extrabold text-4xl sm:text-5xl lg:text-6xl tracking-tight text-center"><a href="https://insta-biter-nyc.vercel.app">
      InstaBiter-NYC
    </a>
    </h1>
    <h1 in:fade={{ delay: 250, duration: 2000, easing: quintInOut }} class="text-slate-400 font-extrabold text-2xl md:text-3xl lg:text-5xl tracking-tight text-center">Track your favorite <br>Instagram food bloggers.</h1>
    <p in:slide={{ delay: 1500, duration: 2000, easing: bounceInOut }} class="mt-6 text-sm md:text-lg text-slate-300 text-center tracking-widest max-w-3xl mx-auto">Frontend: 
      <code class="font-mono font-medium text-lime-500">
        Svelte.js
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        Leaflet.js
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        Tailwindcss
      </code>
    </p>
    <p in:slide={{ delay: 1500, duration: 2000, easing: bounceInOut }} class="mt-6 text-sm md:text-lg text-slate-300 text-center tracking-widest max-w-3xl mx-auto">Backend: 
      <code class="font-mono font-medium text-lime-500">
        Instagram API
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        NoSQL
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        SvelteKit
      </code>
    </p>
    <p in:slide={{ delay: 1500, duration: 2000, easing: bounceInOut }} class="mt-6 text-sm md:text-lg text-slate-300 text-center tracking-widest max-w-3xl mx-auto">Devops:
      <code class="font-mono font-medium text-lime-500">
        GitHub Actions
      </code> |<!--  -->
      <code class="font-mono font-medium text-lime-500">
        Vercel
      </code>
    </p>
  </div>
</div>