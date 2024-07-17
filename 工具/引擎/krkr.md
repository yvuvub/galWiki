
---

styles:["/asset/krkr/css/krkr.css"]

---
## krkr

---

### 存档

krkr引擎的存档文件一般为.ksd格式，其中存储若干对键值对。记录游戏各项设置的存档默认以sc结尾，记录玩家进度的存档默认以su结尾。这些变量将于游戏初始化时，通过loadSystemVariables()函数读取。

![image](/asset/krkr/loadSystemVariables.jpg)

使用十六进制编辑器读取.ksd文件，发现其开头为FE FE XX FF FE。依据XX为00，01，02，.ksd采取了不同的加密方式。可用[kirikiriDescramble](/工具/KirikiriDescrambler.md)解密。
  
  + *tips*
  .ksd文件以FE FE XX FF FE开头，不代表以FE FE XX FF FE的都是krkr存档文件。若确定某文件与krkr引擎制作的游戏有关，且以FE FE XX FF FE开头，即使其扩展名不为.ksd，依旧可试着用kirikiriDescramble解密。  

  ![image](/asset/krkr/解密前.png)

  *解密前*

  ![image](/asset/krkr/解密后.png)

  *解密后，是立绘合成使用的[规则文件](/概念/规则文件.md)*

---