# 原型

```txt
prototype 原型
constructor 构造器
```

```js
function Foo(y) { this.y = y; };
Foo.prototype.x = 10;
FOo.prototype.calculate = function () { ... };
let b = new Foo(20);
let c = new Foo(30);

b.__proto__ === Foo.prototype; // truec.__proto__ === Foo.prototype; // true
```