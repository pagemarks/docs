# Promise

解决callback hell,return,throw能力

[[PromiseState]]: pending / fulfilled / rejected

then(resolved, rejected)

catch()

let promise = new Promise(callback(resolve, reject){}) //立即执行

Promise.resolve(val)
Promise.reject(val)
Promise.all([])      //传递给resolve值为数组,reject为最先reject的值
Promise.race([])     //先决议的p值,不分resolve 和 reject


实现then()方法的任何对象都被称为一个thenable

finally()
无值传递

resolve/reject 只能传递一个参数,需要显式return 传递给下个then

async/await

window unhandledrejection/rejectionhandled 事件捕捉 event (type,promise,reason)
