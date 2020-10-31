# Vue
Concepts and overall introduction to Vue JS

## 5) v-for

<pre>
<code>&ltdiv id="app-4">
  &ltol>
    &ltli v-for="todo in todos">
      {{ todo.text }}
    &lt/li>
  &lt/ol>
&lt/div></code>
</pre>

<pre>
<code>var app4 = new Vue({
  el: '#app-4',
  data: {
    todos: [
      { text: 'Aprender JavaScript' },
      { text: 'Aprender Vue' },
      { text: 'Construir algo increíble' }
    ]
  }
})</code>
</pre>

## 4) v-if

<pre>
<code>&ltdiv id="app-3">
  <span v-if="seen">Ahora me ves</span>
&lt/div></code>
</pre>

<pre>
<code>var app3 = new Vue({
  el: '#app-3',
  data: {
    seen: true
  }
})</code>
</pre>

## 3) v-bind

<pre>
<code>&ltdiv id="app-2">
  &ltspan v-bind:title="message">
    Mueva el mouse sobre mí durante unos segundos
    para ver mi título enlazado dinámicamente.
  &lt/span>
&lt/div></code>
</pre>

<pre>
<code>var app2 = new Vue({
  el: '#app-2',
  data: {
  message: 'Usted cargó esta página el ' + new Date().toLocaleString()
  }
})</code>
</pre>

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
