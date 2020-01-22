setTimeout(fn, time, args?): id
clearTimeout(id)

setInterval(fn, delay, ...args): id
clearInterval(id)
IE9及以下不支持额外参数
fn 可为code string, 不推荐

setImmediate(fn)
IE11/edge 1ms左右,setTimeout 4ms左右

requestAnimationFrame(fn): id
cancelAnimationFrame(id)
浏览器重绘之前触发
