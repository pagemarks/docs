# pwa

## register
```js
navigator.serviceWorker.register('/sw.js')
.then(fn)
.catch(fn)
```
路径作用域,类似cookie

## install

```js
const cache_name = '';
this.addEventListener('install', (e) => {
    this.skipWaiting();
    caches.open(cache_name);
    let cacheResoures=[...urls];
    e.waitUntil(
        caches.open(cache_name).then(cache => {
            cache.addAll(cacheResources)
        })
    )
})
```

event?
caches?

active


fetch
```js
this.addEventListener('fetch', e => {
    e.respondWith(
        caches.match(e.request).then(response => {
            if (response) return response;
            return cache.put(e.request, response.clone())
        })
    )
})
```
caches.match支持第二个参数{ignoreVary: true}.控制url和header一样才匹配


sw更新?

clients? 多tab

message事件通信?

no dom, no window


## manifest.json
```js
{
    "short_name": "",
    "name":"",
    "icons": [{src, type, sizes:'96*96'}],
    "start_url":"",
    "display":"standalone",
    "background-color":"",
    "theme_color":""
}
```

### notify