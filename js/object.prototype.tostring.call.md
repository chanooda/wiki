# Object.prototype.toString.call

기존에 사용되는 `typeof`는 원시타입 이외에는 정확한 구분을 하기 힘들었다. (array, object, function, Date 등)

`Object.prototype.toString.call` 메서드를 사용하면 더 세부적인 타입을 알아낼 수 있다.

<table><thead><tr><th width="512"></th><th></th></tr></thead><tbody><tr><td><code>Object.prototype.toString.call(new Date)</code></td><td><code>[object Date]</code></td></tr><tr><td><code>Object.prototype.toString.call([])</code></td><td><code>[object Array]</code></td></tr><tr><td><code>Object.prototype.toString.call(()=>{})</code></td><td><code>[object Function]</code></td></tr></tbody></table>

