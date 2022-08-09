[CN](README.md) / [EN](README_EN.md)

## mini-vue  [![github](https://img.shields.io/badge/%E5%82%AC%E5%AD%A6%E7%A4%BE-mini--vue-blue)](https://github.com/cuixiaorui/mini-vue)


## Usage

[B 站](https://www.bilibili.com/video/BV1Zy4y1J73E) 提供了视频讲解使用方式



[【课程介绍】](https://www.bilibili.com/video/BV16Z4y1r7Wp?spm_id_from=333.999.0.0)

#### runtime-core

- [x] 支持组件类型
- [x] 支持 element 类型
- [x] 初始化 props
- [x] setup 可获取 props 和 context
- [x] 支持 component emit
- [x] 支持 proxy
- [x] 可以在 render 函数中获取 setup 返回的对象
- [x] nextTick 的实现
- [x] 支持 getCurrentInstance
- [x] 支持 provide/inject
- [x] 支持最基础的 slots
- [x] 支持 Text 类型节点
- [x] 支持 $el api
- [x] 支持 watchEffect


#### reactivity

目标是用自己的 reactivity 支持现有的 demo 运行

- [x] reactive 的实现
- [x] ref 的实现
- [x] readonly 的实现
- [x] computed 的实现
- [x] track 依赖收集
- [x] trigger 触发依赖
- [x] 支持 isReactive
- [x] 支持嵌套 reactive
- [x] 支持 toRaw
- [x] 支持 effect.scheduler
- [x] 支持 effect.stop
- [x] 支持 isReadonly
- [x] 支持 isProxy
- [x] 支持 shallowReadonly
- [x] 支持 proxyRefs

### compiler-core
- [x] 解析插值
- [x] 解析 element
- [x] 解析 text

### runtime-dom
- [x] 支持 custom renderer 


### infrastructure
- [x] support monorepo with pnpm
### todo
- [ ] 实现 runtime-test 可以测试 runtime-core 的逻辑
### build

```shell
pnpm build
```

### example

通过 server 的方式打开 packages/vue/example/\* 下的 index.html 即可

>  推荐使用 [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

### 初始化

#### 流程图
![初始化流程图](https://user-images.githubusercontent.com/12064746/138114565-3e0eecbb-7fd0-4203-bf36-5e5fd8003ce0.png)

> 可加 vx：cuixr1314  获取所有脑图(备注：github mini-vue 领取脑图)
#### 关键函数调用图


![关键函数调用图2](https://user-gold-cdn.xitu.io/2020/6/22/172dc08840e25b42?w=1816&h=934&f=png&s=550722)

> 可以基于函数名快速搜索到源码内容

### update

#### 流程图

![image](https://user-images.githubusercontent.com/12064746/138115157-1f4fb8a2-7e60-412d-96de-12e68eb0288c.png)

#### 关键函数调用图

![image](https://user-images.githubusercontent.com/12064746/138114969-9139e4af-b2df-41b2-a5d9-069d8b41903c.png)


> 可以基于函数名快速搜索到源码内容

