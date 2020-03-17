# 入侵检测第二次作业

创建test.rules文件编写两条规则实现：

- **first packet**
  - **content**:"login"  or "Initial"
  - **dport**=3399
- **second packet**
  - **pcre**:"IPv4AddressPort"string(E.g:123.45.6.7:8080) 
  - dport=3399
- **ouput**
  - msg:"bot founded"
  - sid=1000001
  - 只有两个报文全部匹配时才输出警报

