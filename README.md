最近在做一个wpf端的 websocket客户端。在网上找到了 websocket-csharp 这个项目，后来发现后端websocket 在没有数据推送的情况下过一段时间，会没有数据推送。但是在网页端websocket测试没问题，最后使用wireshark工具发现网页端多了一个keep-alive，用wireshark检测发现没有开启keep-alive, 最后在源码中开启keep-alive模式就没问题了。大家可以下载代码试试！
