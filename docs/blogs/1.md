# 互联网安全

- 互联网安全架构.docx

## 信息加密

### 单向加密-不可逆

- MD5,SHA......

- 应用场景：验证信息，密码加密

### 双向加密-可逆

#### 对称加密

- DES,3DES,AES......
- 应用场景：海量数据加密，服务器内部信息传输，数据库敏感信息加密

#### 非对称加密 

- RSA、Elgamal、背包算法......
- 应用场景：数字签名，客户端和服务端通信https

### 数据库数据加密

- 采用非对称加密算法管理对称算法的密钥，然后用对称加密算法加密数据。

  这样我们就集成了两类加密算法的优点，既实现了加密速度快的优点

  ，又实现了安全方便管理密钥的优点。

## 秘钥管理

- 生成秘钥文件
  1. 上传至单独服务器保存
  2. 保存到管理者电脑，采用BitLocker驱动加密保管
  3. 或者其它存储媒介
- 数字认证 CA ......

### 管理工具

- [Java  keytool](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/keytool.html)  是密钥和证书管理工具

- 介绍

  Keytool 是一个Java数据证书的管理工具 ,Keytool将密钥（key）和证书（certificates）存在一个称为keystore的文件中在keystore里，包含两种数据:密钥实体（Key entity）-密钥（secret key）或者是私钥和配对公钥（采用非对称加密）可信任的证书实体（trusted certificate entries）-只包含公钥.
  
- [keytool 可视化工具](https://www.jb51.net/softs/542444.html)        

-  [可视化工具简单使用教程](https://blog.csdn.net/wyx100/article/details/46485935)

- 参考文章
  1. [官网文档](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/keytool.html)
  2. [常用的Java Keytool Keystore命令](https://www.chinassl.net/ssltools/keytool-commands.html)
  3. [使用Java自带的keytool工具生成RSA非对称密钥证书，并导出公钥文件](https://blog.csdn.net/freezingxu/article/details/71547485)


