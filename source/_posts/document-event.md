---
title: document的事件详解
date: 2022-11-03 08:52:20
categories:
  - HTML
tags: 
  - document
  - event
---

## document的一些事件

最近想做一下资源加载的监听所以又去了解了下，有些事件不做基础建设的工作有时候也就一笔带过用用就又忘了，所以想记一记加深下印象。

### readystatechange事件

```typescript
document.addEventListener('readystatechange', () => {});
xhr.addEventListener('readystatechange', () => {});
```

readystatechange事件会记录被监听对象的状态的变更，经过测试挂载在window下不生效。事件分为多个状态挂在到目标的readyState对象上
+ uninitialized（未初始化）
+ loading（正在加载）
+ loaded (加载完毕)
+ interactive (交互)
+ complete (完成)
在实际的的使用中并不完全都会出现这些状态，具体根据dom能支持的行为输出。行为不是很稳定

### loadstart事件
```typescript
测试
```
