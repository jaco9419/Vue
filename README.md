# Vue
Concepts and overall introduction to Vue JS

## 2) Start

### In index.js:
<pre>
<code>var app = new Vue({
  el: '#app',
  data: {
  message: 'Hola Vue!'
  }
})</code>
</pre>

### In index.html:
<pre>
<code>&ltdiv id="app">
{{ message }}
&lt/div>
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
<script src="index.js"></script></code>
</pre>

## 1) CDN
For prototyping or learning purposes, you can use the latest version with:

<pre>
<code><script src="https://cdn.jsdelivr.net/npm/vue@2.6.12/dist/vue.js"></script></code>
</pre>

For production, we recommend linking to a specific version number and build to avoid unexpected breakage from newer versions:

<pre>
<code><script src="https://cdn.jsdelivr.net/npm/vue@2.6.12"></script></code>
</pre>
If you are using native ES Modules, there is also an ES Modules compatible build:

<pre>
<code><script type="module">
  import Vue from 'https://cdn.jsdelivr.net/npm/vue@2.6.12/dist/vue.esm.browser.js'
</script></code>
</pre>
