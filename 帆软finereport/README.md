前置基础
---


相关漏洞
---

### CNVD-2021-34467 v9 文件上传


利用研究
---

### 密码解密

> python

密码配置文件
```
\WEB-INF\resources\privilege.xml
```
获取加密后的密文

![image](https://user-images.githubusercontent.com/55024146/129508186-d55dace1-7218-4dd9-9848-b33c842e1005.png)

反编译jar包获取加密代码逻辑

![image](https://user-images.githubusercontent.com/55024146/129508634-ee7e2498-e31f-49d9-a77c-e14a60794b9c.png)


解密脚本
![image](https://user-images.githubusercontent.com/55024146/159114641-26d5a937-b5e7-4f0d-bb44-cf5864279c05.png)


> java

- 获取加解密逻辑姿势同上

```shell
java -jar .\X-FineReport.jar --encode pen4uin
java -jar .\X-FineReport.jar --decode ___0063002b0064003b001100bc0045
```

![image](https://user-images.githubusercontent.com/55024146/159114652-70a84da5-327a-4b2d-8077-bb18aef87a2c.png)
