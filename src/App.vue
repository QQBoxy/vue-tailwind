<script setup>
import { ref, onMounted } from 'vue';
// import qqboxyImportUrl from './assets/images/qqboxy.jpg';
const qqboxyUrl = ref("");
const qqboxyNewUrl = ref("");

onMounted(() => {
  qqboxyUrl.value = "./assets/images/qqboxy.jpg";
  qqboxyNewUrl.value = new URL('./assets/images/qqboxy.jpg', import.meta.url).href;
});
</script>

<template>
  <h1>Background Image</h1>
  <h2>Static</h2>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="bg bg1"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 1</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Static</span>
        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#CSS
          Class</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;template&gt;
  <span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"bg bg1"</span>&gt;</span>1<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span></span>
&lt;/template&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">style</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">scoped</span>&gt;</span><span style="color: rgb(0, 0, 0); font-weight: 400;">
<span style="color: rgb(0, 0, 0); font-weight: 400;">.bg</span> {
  <span style="color: rgb(163, 21, 21); font-weight: 400;">width</span>: <span style="color: rgb(0, 0, 0); font-weight: 400;">200px</span>;
  <span style="color: rgb(163, 21, 21); font-weight: 400;">height</span>: <span style="color: rgb(0, 0, 0); font-weight: 400;">200px</span>;
  <span style="color: rgb(163, 21, 21); font-weight: 400;">background-size</span>: contain;
  <span style="color: rgb(163, 21, 21); font-weight: 400;">background-repeat</span>: no-repeat;
  <span style="color: rgb(163, 21, 21); font-weight: 400;">background-position</span>: center;
}

<span style="color: rgb(0, 0, 0); font-weight: 400;">.bg1</span> {
  <span style="color: rgb(163, 21, 21); font-weight: 400;">background-image</span>: <span style="color: rgb(0, 0, 255); font-weight: 400;">url</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">'./assets/images/qqboxy.jpg'</span>);
}
</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">style</span>&gt;</span></span></pre>
    </div>
  </div>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="w-[200px] h-[200px] bg-contain bg-no-repeat bg-center bg1"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 2</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Static</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#CSS
          Class</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;template&gt;
  <span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[200px] h-[200px] bg-contain bg-no-repeat bg-center bg1"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span></span>
&lt;/template&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">style</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">scoped</span>&gt;</span><span style="color: rgb(0, 0, 0); font-weight: 400;">
<span style="color: rgb(0, 0, 0); font-weight: 400;">.bg1</span> {
  <span style="color: rgb(163, 21, 21); font-weight: 400;">background-image</span>: <span style="color: rgb(0, 0, 255); font-weight: 400;">url</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">'./assets/images/qqboxy.jpg'</span>);
}
</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">style</span>&gt;</span></span></pre>
    </div>
  </div>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="w-[200px] h-[200px] bg-contain bg-no-repeat bg-center bg-[url('./assets/images/qqboxy.jpg')]"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 3</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Static</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
      </div>
      <pre style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;template&gt;
  <span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[200px] h-[200px] bg-contain bg-no-repeat bg-center bg-[url('./assets/images/qqboxy.jpg')]"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span></span>
&lt;/template&gt;</pre>
    </div>
  </div>

  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="w-[200px] h-[200px] bg-contain bg-no-repeat bg-center" :class="`bg-[url('${qqboxyImportUrl}')]`"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 4</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Static</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
      </div>

    </div>
  </div>


  <h2>Dynamic</h2>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div
        style="width: 200px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"
        :style="{ 'background-image': `url('${qqboxyNewUrl}')` }"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 1</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Dynamic</span>
        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#CSS
          Style</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyNewUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyNewUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(0, 0, 255); font-weight: 400;">new</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">URL</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">'./assets/images/qqboxy.jpg'</span>, <span style="color: rgb(0, 0, 255); font-weight: 400;">import</span>.<span style="color: rgb(0, 0, 0); font-weight: 400;">meta</span>.<span style="color: rgb(0, 0, 0); font-weight: 400;">url</span>).<span style="color: rgb(0, 0, 0); font-weight: 400;">href</span>;
});
&lt;/script&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span>
  <span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>
    <span style="color: rgb(255, 0, 0); font-weight: 400;">style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"width: 200px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"</span>
    <span style="color: rgb(255, 0, 0); font-weight: 400;">:style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ 'background-image': `url('${qqboxyNewUrl}')` }"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span>
<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span></span></pre>
    </div>
  </div>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div
        style="width: 200px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"
        :style="{ 'background-image': 'url(\'' + qqboxyNewUrl + '\')' }"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 2</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Dynamic</span>
        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#CSS
          Style</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyNewUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyNewUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(0, 0, 255); font-weight: 400;">new</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">URL</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">'./assets/images/qqboxy.jpg'</span>, <span style="color: rgb(0, 0, 255); font-weight: 400;">import</span>.<span style="color: rgb(0, 0, 0); font-weight: 400;">meta</span>.<span style="color: rgb(0, 0, 0); font-weight: 400;">url</span>).<span style="color: rgb(0, 0, 0); font-weight: 400;">href</span>;
});
&lt;/script&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span>
  <span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"width: 200px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">:style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ 'background-image': 'url(\'' + qqboxyNewUrl + '\')' }"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span>
<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span></span></pre>
    </div>
  </div>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="w-[200px] h-[200px] bg-contain bg-no-repeat bg-center" :class="`bg-[url('${qqboxyUrl}')]`"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 3</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Dynamic</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(163, 21, 21); font-weight: 400;">"./assets/images/qqboxy.jpg"</span>;
});
&lt;/script&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span>
  <span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[200px] h-[200px] bg-contain bg-no-repeat bg-center"</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">:class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"`bg-[url('${qqboxyUrl}')]`"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span>
<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span></span></pre>
    </div>
  </div>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="w-[200px] h-[200px] bg-contain bg-no-repeat bg-center" :class="'bg-[url(\'' + qqboxyUrl + '\')]'">
      </div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 4</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Dynamic</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(163, 21, 21); font-weight: 400;">"./assets/images/qqboxy.jpg"</span>;
});
&lt;/script&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span>
  <span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[200px] h-[200px] bg-contain bg-no-repeat bg-center"</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">:class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"'bg-[url(\'' + qqboxyUrl + '\')]'"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span>
<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span></span></pre>
    </div>
  </div>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="w-[200px] h-[200px] bg-contain bg-no-repeat bg-center"
        :class="{ [`bg-[url('${qqboxyUrl}')]`]: true }"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 5</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Dynamic</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(163, 21, 21); font-weight: 400;">"./assets/images/qqboxy.jpg"</span>;
});
&lt;/script&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span>
  <span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[200px] h-[200px] bg-contain bg-no-repeat bg-center"</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">:class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ [`bg-[url('${qqboxyUrl}')]`]: true }"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span>
<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span></span></pre>
    </div>
  </div>
  <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">
      <div class="w-[200px] h-[200px] bg-contain bg-no-repeat bg-center"
        :class="{ ['bg-[url(\'' + qqboxyUrl + '\')]']: true }"></div>
    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 6</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Dynamic</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
      </div>
      <pre
        style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(163, 21, 21); font-weight: 400;">"./assets/images/qqboxy.jpg"</span>;
});
&lt;/script&gt;
<span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span>
  <span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[200px] h-[200px] bg-contain bg-no-repeat bg-center"</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">:class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ ['bg-[url(\'' + qqboxyUrl + '\')]']: true }"</span>&gt;</span><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span>
<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">template</span>&gt;</span></span></pre>
    </div>
  </div>

  <!-- <div
    class="max-w w-full lg:max-w-full lg:flex border-r border-b border-l border-gray-400 lg:border-l-0 lg:border-t lg:border-gray-400 bg-white rounded-b lg:rounded-b-none lg:rounded-r lg:mb-5">
    <div class="w-[200px]">

    </div>
    <div class="w-full p-4 flex flex-col justify-between leading-normal">
      <div class="text-gray-900 font-bold text-xl mb-2">Method 1</div>
      <div class="pt-2 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Dynamic</span>
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#Tailwind</span>
      </div>

    </div>
  </div> -->

</template>

<style scoped>
h1 {
  font-size: xx-large;
  padding: 10px;
}

h2 {
  font-size: x-large;
  padding: 10px;
}

h3 {
  font-size: large;
  padding: 10px;
}

.bg {
  width: 200px;
  height: 200px;
  background-size: contain;
  background-repeat: no-repeat;
  background-position: center;
}

.bg1 {
  background-image: url('./assets/images/qqboxy.jpg');
}

pre {
  white-space: pre-wrap;
  word-wrap: break-word;
}
</style>
