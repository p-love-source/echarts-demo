
### 实现Vue的数据劫持
```
vue2.x Object.defineProperty
vue3.0 Proxy
```
### 优点
```

1、性能更好
Object.defineProperty只能监听属性，而Proxy能监听整个对象，省去对非对象或数组类型的劫持，也能做到监听。

vue2.x是对对象每一个属性进行Object.defineProperty。
vue3.0 proxy ==> 省去了遍历元素。

2、Object.defineProperty不能监测到数组变化

```