# web_im_ajax
web即时聊天(ajax长轮询方式实现)

功能介绍：
1.对话双方都在线（浏览器没有关闭的情况下），对话即时推算．
２．当一方不在线时，支持离线发送消息．当离线方上线时，会自动接收离线消息．

功能特点：
１．采用ajax＋长轮询，简单易懂．
２．减少ajax发起的无效http连接．
３．使用确认机制来确保客户端收到信息．
４．使用超时机制来确保用户离线时，关闭连接．

客户端使用方式:
假如AB两人对话,A的UID为1,B的UID为2.

A发起的url为
http://domain/client.php?from=1&to=2
B发起的url为
http://domain/client.php?from=2&to=1
