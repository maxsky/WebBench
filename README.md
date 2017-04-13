# WebBench
Web Bench 是一个非常简单的用于 WWW 或代理服务器的基准测试工具。使用 fork() 模拟多个客户端，并且可以使用 HTTP/0.9-HTTP/1.1 的请求。这个基准测试是不太现实的，但它可以测试，如果你的 httpd 确定能实时处理多个客户端（尝试运行一些CGI）而不会使您的机器宕机的话。显示 页面/分钟 和 字节/秒，可以用 -f 选项在更积极的模式下使用。

webbench [选项]... URL
  -f|--force               不等待服务器答复
  -r|--reload              发送重载请求 - 参数: no-cache
  -t|--time <sec>          运行基准测试 <sec> 秒. 默认 30
  -p|--proxy <server:port> 使用代理服务器进行请求
  -c|--clients <n>         立即运行 <n> 个 HTTP 客户端. 默认 1
  -9|--http09              使用 HTTP/0.9 请求方式
  -1|--http10              使用 HTTP/1.0 协议
  -2|--http11              使用 HTTP/1.1 协议
  --get                    使用 GET 请求方法
  --head                   使用 HEAD 请求方法
  --options                使用 OPTIONS 请求方法
  --trace                  使用 TRACE 请求方法
  -?|-h|--help             显示帮助信息
  -V|--version             显示程序版本
