<script setup>
const features = [
  {
    title: 'Customizable Control Interfaces',
    description:
      'Craft your control interface using Vue, web components, or traditional HTML + JavaScript.',
    icon: 'bx:bxs-briefcase',
  },
  {
    title: 'Efficient Static Rendering',
    description:
      'Our system renders your entire interface to static HTML, eliminating unnecessary JavaScript from the final output.',
    icon: 'bx:bxs-window-alt',
  },
  {
    title: 'Dynamic Component Loading',
    description:
      'Require dynamic components? Our platform can dynamically load interactive elements as needed, enhancing user experience.',
    icon: 'bx:bxs-data',
  },
  {
    title: 'Versatile Integration',
    description:
      'Our solution seamlessly integrates with TypeScript, Scoped CSS, CSS Modules, Sass, Tailwind, Markdown, MDX, and other essential npm packages.',
    icon: 'bx:bxs-bot',
  },
  {
    title: 'Optimized for Search Engines',
    description:
      'Enjoy automatic generation of sitemaps, RSS feeds, pagination, and collections for effortless SEO and content syndication.',
    icon: 'bx:bxs-file-find',
  },
  {
    title: 'Thriving Community Support',
    description:
      'Join our vibrant community of contributors who are continually enhancing our platform with their invaluable contributions.',
    icon: 'bx:bxs-user',
  },
]
</script>

<template>
  <div class="mt-16 md:mt-0">
    <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight">
      Everything you need to control your "Bagger"
    </h2>
    <p class="text-lg mt-4 text-slate-600">
      Our platform offers a wide range of features to help you manage your
      "Bagger" with ease.
    </p>
  </div>

  <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
    <div v-for="item of features" class="flex gap-4 items-start">
      <div class="mt-1 bg-black rounded-full p-2 w-8 h-8 shrink-0">
        <Icon class="text-white" :name="item.icon" />
      </div>
      <div>
        <h3 class="font-semibold text-lg">{{ item.title }}</h3>
        <p class="text-slate-500 mt-2 leading-relaxed">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
