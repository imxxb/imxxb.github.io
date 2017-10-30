---
title: Dispatcher.js 代码中类型申明标记是什么？
layout: post
---

在阅读flux的中源代码时候遇到一些奇怪的标记

```javascript

class Dispatcher<TPayload> {
  _callbacks: {[key: DispatchToken]: (payload: TPayload) => void};
  _isDispatching: boolean;
  _isHandled: {[key: DispatchToken]: boolean};
  _isPending: {[key: DispatchToken]: boolean};
  _lastID: number;
  _pendingPayload: TPayload;
  //以下省略
}

```

查询了issues的讨论[Add flow types to dispatcher #243](https://github.com/facebook/flux/pull/243) 知道了是[flow](http://flowtype.org)。
