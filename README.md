# mk184
React源码深度解析 高级前端工程师必备技能
React源码深度解析 高级前端工程师必备技能
[![下载地址](https://img.mukewang.com/szimg/5fce053d09e4a2d405400304.jpg "下载地址")](https://51xueit.vip "下载地址")
[下载地址](https://51xueit.vip "下载地址")
### 第1章 课程导学 

#### 对课程整体进行讲解。
1-1 课程导学 (11:08)


### 第2章 基础知识 React API 一览 

#### React主要API介绍，在这里你能了解它的用法，为下一章源码分析打基础。
2-1 准备工作 (11:07)

2-2 JSX到JavaScript的转换 (07:17)

2-3 react-element (11:08)

2-4 react-component (08:46)

2-5 react-ref (06:40)

2-6 forward-ref (06:55)

2-7 context (10:26)

2-8 concurrent-mode (09:32)

2-9 suspense-and-lazy (09:32)

2-10 hooks (11:02)

2-11 children (22:34)

2-12 others (08:28)


### 第3章 React中的更新 

#### 主要讲解React创建更新中的主要两种方式ReactDOM.render和setState，他们具体做了什么。
3-1 react-dom-render (25:41)

3-2 react-fiber-root (10:45)

3-3 react-fiber (12:50)

3-4 react-update-and-updateQueue (14:24)

3-5 react-expiration-time (15:50)

3-6 different-expirtation-time (11:29)

3-7 react-setState-forceUpdate (06:55)


### 第4章 Fiber Scheduler

#### 创建更新之后，找到Root然后进入调度，同步和异步操作完全不同，实现更新分片的性能优化。
4-1 总结流程概览 (20:04)

4-2 scheduleWork (22:13)

4-3 requestWork (09:49)

4-4 batchedUpdates (15:12)

4-5 reactScheduler（1） (12:54)

4-6 reactScheduler（2） (12:39)

4-7 reactScheduler（3） (20:10)

4-8 reactScheduler（4） (14:19)

4-9 performWork (18:43)

4-10 renderRoot (14:00)

4-11 最后补充 (11:41)


### 第5章 各类组件的Update

#### 讲解10多种不同类型的组件的更新过程，以及如何遍历节点形成新的Fiber树
5-1 入口和优化 (17:47)

5-2 FunctionalComponent的更新 (07:06)

5-3 reconcilerChildren (26:36)

5-4 reconcilerChildren-array (23:57)

5-5 updateClassComponent (27:01)

5-6 ClassComponent的更新 (09:10)

5-7 IndeterminateComponent组件类型和其更新过程 (07:03)

5-8 HostRoot的更新 (05:11)

5-9 HostComponent和HostText的更新 (08:29)

5-10 Poratl组件的更新 (05:11)

5-11 ForwardRef的更新 (02:54)

5-12 Mode组件的更新 (04:55)

5-13 Memo组件的更新 (09:16)


### 第6章 完成节点任务

#### 完成节点更新之后完成节点的创建，并提供优化到最小幅度的DOM更新列表
6-1 completeUnitOfWork的整体流程和意义 (24:12)

6-2 重设childExpirationTime (06:54)

6-3 completWork具体做了什么 (04:00)

6-4 初次渲染中completeWork对于DOM节点的创建和appendAllChild算法 (16:50)

6-5 初次渲染中如何进行DOM节点属性初始化操作 (14:22)

6-6 更新DOM时进行的diff判断 (08:24)

6-7 completeWork阶段对于HostText的更新 (03:21)

6-8 renderRoot中对于错误的处理 (14:03)

6-9 unwindWork以及React中的错误处理 (15:02)


### 第7章 commitRoot

#### 根据更新列表最小幅度的改变DOM，实现UI的更新。
7-1 commitRoot的总体工作内容 (11:31)

7-2 invokeGuardedCallback开发时的帮助方法 (13:44)

7-3 commitRoot第一个操作-获取快照 (04:57)

7-4 commitAllHostEffects总体做了哪些事情 (06:23)

7-5 commitPlacement插入新的子节点的操作 (17:31)

7-6 commitWork更新节点属性的过程 (11:50)

7-7 commitWork删除节点的操作过程 (17:47)

7-8 commitLifecycles调用生命周期方法 (11:23)


### 第8章 功能详解：基础

#### 各种贯穿于更新和提交阶段的功能，他们在哪里发挥作用，又是如何实现功能的
8-1 context-stack (12:21)

8-2 遗留context-api的实现过程（1） (17:06)

8-3 遗留context-api的实现过程（2） (15:19)

8-4 新context的实现 (22:36)

8-5 ref的实现过程 (09:25)

8-6 hydrate-是否需要hydrate的判断 (06:44)

8-7 hydrate-更新开始判断节点是否可以hydrate (11:35)

8-8 hydrate-再completeWork中复用可hydrate的节点 (16:09)

8-9 event事件系统初始化-注入平台事件插件 (20:12)

8-10 event事件监听的过程 (14:24)

8-11 event-事件触发的过程 (21:16)

8-12 event-事件对象的生产过程 (19:40)

8-13 event查漏补缺 (09:58)


### 第9章 suspense and priority

#### Suspense作为下一个React的杀手功能，他又是如何实现异步渲染的呢？
9-1 优先级和任务挂起的含义（1） (14:48)

9-2 优先级和任务挂起的含义（2） (14:35)

9-3 两个expirationTime的不同作用 (11:55)

9-4 Suspense组件同步模式下的更新 (24:12)

9-5 Suspense组件同步渲染模式补充 (08:43)

9-6 Suspense组件异步模式下的更新 (20:24)

9-7 retrySuspendedWork所做的事情 (08:35)


### 第10章 功能详解：Hooks

#### Hooks颠覆原先的React组件开发模式，提供更小粒度的更新以及更加适合解耦的API。
10-1 什么是Hooks以及他的用法 (22:29)

10-2 Hooks的定义以及执行前后的准备和重置 (17:54)

10-3 useState的实现原理和注意事项（1） (13:38)

10-4 useState的实现原理和注意事项（2） (13:59)

10-5 useEffect和useLayoutEffect的实现原理和区别 (23:37)

10-6 其他Hooks的实现 (08:20)


### 第11章 课程总结

#### 对课程整体进行回顾，以及总结。
11-1 课程总结 (12:05)


[下载地址](https://51xueit.vip "下载地址")
