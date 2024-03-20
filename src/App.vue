<script setup>
import { ref, onMounted } from 'vue';
const qqboxyUrl = ref("");
const qqboxyNewUrl = ref("");

onMounted(() => {
  qqboxyUrl.value = "./assets/images/qqboxy.jpg";
  qqboxyNewUrl.value = new URL('./assets/images/qqboxy.jpg', import.meta.url).href;
});
</script>

<template>
  <div class="mb-10 border-red-500 border-2">
    <h1>CSS Style</h1>
    <br />
    <pre style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyNewUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyNewUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(0, 0, 255); font-weight: 400;">new</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">URL</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">'./assets/images/qqboxy.jpg'</span>, <span style="color: rgb(0, 0, 255); font-weight: 400;">import</span>.<span style="color: rgb(0, 0, 0); font-weight: 400;">meta</span>.<span style="color: rgb(0, 0, 0); font-weight: 400;">url</span>).<span style="color: rgb(0, 0, 0); font-weight: 400;">href</span>;
});
&lt;/script&gt;</pre>
    <br />
    <div
      style="width: 300px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"
      :style="{ 'background-image': `url('${qqboxyNewUrl}')` }">1-1</div>
    <pre style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;template&gt;
  <span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"width: 300px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">:style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ 'background-image': `url('${qqboxyNewUrl}')` }"</span>&gt;</span>1-1<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span></span>
&lt;/template&gt;</pre>
    <br />
    <div
      style="width: 300px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"
      :style="{ 'background-image': 'url(\'' + qqboxyNewUrl + '\')' }">1-2</div>
    <pre style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;template&gt;
  <span style="color: rgb(0, 0, 0); font-weight: 400;"><span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"width: 300px; height: 200px; background-size: contain; background-repeat: no-repeat; background-position: center;"</span> <span style="color: rgb(255, 0, 0); font-weight: 400;">:style</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ 'background-image': 'url(\'' + qqboxyNewUrl + '\')' }"</span>&gt;</span>1-2<span style="color: rgb(0, 0, 255); font-weight: 400;">&lt;/<span style="color: rgb(0, 0, 255); font-weight: 400;">div</span>&gt;</span></span>
&lt;/template&gt;</pre>
  </div>
  <div class="mb-10 border-blue-500 border-2">
    <h1>CSS Class</h1>
    <br />
    <div class="bg bg1">1</div>
    <pre
      style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;div <span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"bg bg1"</span>&gt;<span style="color: rgb(0, 0, 0); font-weight: 400;">1</span>&lt;/div&gt;</pre>
    <pre style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;style scoped&gt;
.<span style="color: rgb(0, 0, 0); font-weight: 400;">bg</span> {
  <span style="color: rgb(255, 0, 0); font-weight: 400;">width</span>: 300px;
  <span style="color: rgb(255, 0, 0); font-weight: 400;">height</span>: 200px;
  background-<span style="color: rgb(255, 0, 0); font-weight: 400;">size</span>: contain;
  background-<span style="color: rgb(255, 0, 0); font-weight: 400;">repeat</span>: no-repeat;
  background-<span style="color: rgb(255, 0, 0); font-weight: 400;">position</span>: center;
}

.<span style="color: rgb(0, 0, 0); font-weight: 400;">bg1</span> {
  background-<span style="color: rgb(255, 0, 0); font-weight: 400;">image</span>: <span style="color: rgb(163, 21, 21); font-weight: 400;">url</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">'./assets/images/qqboxy.jpg'</span>);
}
&lt;/style&gt;</pre>
  </div>
  <div class="mb-10 border-green-500 border-2">
    <h1>Tailwind</h1>
    <br />
    <pre style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;script setup&gt;
<span style="color: rgb(0, 0, 255); font-weight: 400;">import</span> { ref, onMounted } <span style="color: rgb(0, 0, 255); font-weight: 400;">from</span> <span style="color: rgb(163, 21, 21); font-weight: 400;">'vue'</span>;
<span style="color: rgb(0, 0, 255); font-weight: 400;">const</span> qqboxyUrl = <span style="color: rgb(163, 21, 21); font-weight: 400;">ref</span>(<span style="color: rgb(163, 21, 21); font-weight: 400;">""</span>);
<span style="color: rgb(163, 21, 21); font-weight: 400;">onMounted</span>(<span style="color: rgb(0, 0, 0); font-weight: 400;">() =&gt;</span> {
  qqboxyUrl.<span style="color: rgb(0, 0, 0); font-weight: 400;">value</span> = <span style="color: rgb(163, 21, 21); font-weight: 400;">"./assets/images/qqboxy.jpg"</span>;
});
&lt;/script&gt;</pre>
    <br />
    <div class="w-[300px] h-[200px] bg-contain bg-no-repeat bg-center bg-[url('./assets/images/qqboxy.jpg')]">1</div>
    <pre
      style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;div <span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[300px] h-[200px] bg-contain bg-no-repeat bg-center bg-[url('./assets/images/qqboxy.jpg')]"</span>&gt;<span style="color: rgb(0, 0, 0); font-weight: 400;">1</span>&lt;/div&gt;</pre>
    <br />
    <div class="w-[300px] h-[200px] bg-contain bg-no-repeat bg-center" :class="`bg-[url('${qqboxyUrl}')]`">2-1</div>
    <pre
      style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;div <span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[300px] h-[200px] bg-contain bg-no-repeat bg-center"</span> :<span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"`bg-[url('${qqboxyUrl}')]`"</span>&gt;<span style="color: rgb(0, 0, 0); font-weight: 400;">2</span>-<span style="color: rgb(0, 0, 0); font-weight: 400;">1</span>&lt;/div&gt;</pre>
    <br />
    <div class="w-[300px] h-[200px] bg-contain bg-no-repeat bg-center" :class="'bg-[url(\'' + qqboxyUrl + '\')]'">2-2
    </div>
    <pre
      style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;div <span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[300px] h-[200px] bg-contain bg-no-repeat bg-center"</span> :<span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"'bg-[url(\'' + qqboxyUrl + '\')]'"</span>&gt;<span style="color: rgb(0, 0, 0); font-weight: 400;">2</span>-<span style="color: rgb(0, 0, 0); font-weight: 400;">2</span>&lt;/div&gt;</pre>
    <br />
    <div class="w-[300px] h-[200px] bg-contain bg-no-repeat bg-center" :class="{ [`bg-[url('${qqboxyUrl}')]`]: true }">
      3-1</div>
    <pre
      style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;div <span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[300px] h-[200px] bg-contain bg-no-repeat bg-center"</span> :<span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ [`bg-[url('${qqboxyUrl}')]`]: true }"</span>&gt;<span style="color: rgb(0, 0, 0); font-weight: 400;">3</span>-<span style="color: rgb(0, 0, 0); font-weight: 400;">1</span>&lt;/div&gt;</pre>
    <br />
    <div class="w-[300px] h-[200px] bg-contain bg-no-repeat bg-center"
      :class="{ ['bg-[url(\'' + qqboxyUrl + '\')]']: true }">3-2</div>
    <pre
      style="font-family:monospace;color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); font-weight: 400; ">&lt;div <span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"w-[300px] h-[200px] bg-contain bg-no-repeat bg-center"</span> :<span style="color: rgb(0, 0, 255); font-weight: 400;">class</span>=<span style="color: rgb(163, 21, 21); font-weight: 400;">"{ ['bg-[url(\'' + qqboxyUrl + '\')]']: true }"</span>&gt;<span style="color: rgb(0, 0, 0); font-weight: 400;">3</span>-<span style="color: rgb(0, 0, 0); font-weight: 400;">2</span>&lt;/div&gt;</pre>
  </div>
</template>

<style scoped>
.bg {
  width: 300px;
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
