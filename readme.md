## postMessage 两个页面通信

### 如何跑起来

- 进入 website1 目录

- http-server -c-1 -p 8082

- 进入 website2 目录

- http-server -c-1 -p 8083

- 访问 http://127.0.0.1:8082/page1.html

- 点击 go to page2 按钮

- 

### 核心

- 新增 message 事件、触发 message 事件是不同页面的同一个 window 上操作

- 「不同页面的同一个 window 上操作」如何理解?

    page1 想新增 message 事件，这很简单，直接在 page1 的 window 正常注册事件即可，搜索 「page1 新增监听事件」

    但是想在 page2 触发 message 事件，那么需要在 page2 得到 page1 的 window，然后使用这个 window 触发事件，搜索「在 page2 得到 page1 的引用」、「在 page1 得到 page2 的引用」，


