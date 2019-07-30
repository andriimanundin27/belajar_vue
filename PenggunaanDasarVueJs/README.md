## Cara Menggunakan Vue
- Download file vue.js dan memanggilnya dalam file HTML
- Langsung memanggil vue.js melalui url CDN cdnjs, unpkg, jsDelivr dan
- menggunakan Node.js (Vue CLI) `tidak cocok untuk pemula`

### contoh CDN

> <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>

> <script src="https://cdn.jsdelivr.net/npm/vue"></script>

### inti dari vue.js
```
<div id="app">
  {{ message }}
</div>
```

```
var app = new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue!'
  }
})
```

### teks reaktif untuk menampilkan pesan ketika cursor diatas teks

```
<div id="app">
    <span v-bind:title="message">{{ message }}</span>
 </div>
```

```
<div id="app">
    <span :title="message">{{ message }}</span>
</div>
```

`v-bind` adalah atribut direktif, biasa disingkat `v-` atau `:` (atribut khusus vue.js) atau (data binding)

