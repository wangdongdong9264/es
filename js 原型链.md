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

```md
1. __proto__ 是原型链查询中实际用到的，它总是指向 prototype；
2. prototype 在定义构造函数时自动创建，它总是被 __proto__ 所指。
```