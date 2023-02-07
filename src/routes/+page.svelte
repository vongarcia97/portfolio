<script>
  import profilePhoto from '$lib/assets/profilePhoto.gif';
  import { fly, scale, slide } from 'svelte/transition';
  import { quintInOut } from 'svelte/easing';

  const bioLines = [
    'Software Developer based in NYC, ',
    'with prior experience in healthcare. ',
    'An active member of GitFitCode, ',
    'a professional community of lifelong learners ',
    'and hub for knowledge sharing and collaboration. ',
    'Always excited to work with great people ',
    'developing high-impact projects that solve real-world problems!'
  ]

  const techStack = [
    'JavaScript ES6+ | Python | HTML5 | CSS',
    'React.js | Svelte.js | Tailwindcss | Scss | Webpack',
    'Node.js | Express.js | Next.js | SvelteKit | WebSockets',
    'Auth & OAuth | SQL | NoSQL | XML | REST | JSON',
    'NPM | Git | AWS EC2, S3, IAM, Elastic Beanstalk | Vercel'
  ];
</script>

<figure class="bg-transparent h-full">
  <div class="avatar w-full justify-center pt-10">
    <div class="w-32 md:w-64 rounded-full" in:scale={{
          delay: 250,
          duration: 1000,
          easing: quintInOut
        }}>

      <img alt="user-avatar" src={profilePhoto}/>
    </div>
  </div>
  <div id="info-container" class="w-full text-center font-medium pt-3 md:pt-5">
    <div class="font-semibold tracking-wide text-xl md:text-3xl">
      Von Garcia
    </div>
    <div class="text-slate-300 dark:text-slate-300 text-lg md:text-xl">
      Full Stack Software Engineer
    </div>
    <div class="text-slate-400 dark:text-slate-400 text-md md:text-lg">
      New York, NY
    </div>
  </div>
  <div class="pt-10 text-center">
    {#each bioLines as line, i}
    <div class="px-2 lg:px-24">
      <span class="text-md md:text-xl lg:text-2xl font-medium align-middle "
        in:fly={{
          y: -100 * i,
          delay: 250 * i,
          duration: 2500,
          easing: quintInOut
        }}
      >
        {line}
      </span>
    </div>
    {/each}
    <!-- svelte-ignore a11y-structure -->
    <figcaption class="font-medium">
      <div id="technologies-container" class="pt-24">
        <h1 class="text-bold text-lg md:text-2xl lg:text-3xl pb-4" in:scale={{
          delay: 3000,
          duration: 2000,
          easing: quintInOut
        }}>
        TECHNOLOGIES SNAPSHOT
        </h1>
        {#each techStack as tech, i}
          <p class="text-slate-300 dark:text-slate-300 text-xs md:text-lg px-4" in:slide={{
          delay: 1000 * i + 3000,
          duration: 2000,
          easing: quintInOut
        }}>
            {tech}
          </p>
        {/each}
      </div>
    </figcaption>
  </div>
</figure>