dat文件本质是zip，随便一个解压工具就能解，密码是IrsysPack_CipherKey  
CstxPack：  
提取cstx文字  
示例：cstxpack.exe -e -op C:\Users\(用户名)\Desktop\input -sp C:\Users\(用户名)\Desktop\output -text omsg -cp 65001 -com true  
ToolForAtlas：  
还原块状图片及导回，atx文件本身是不加密的zip文件，ToolForAtlas原理是使用json里的数据将图片还原  
示例：ToolForAtlas -x [json所在文件夹]   
