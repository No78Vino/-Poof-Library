# gihub:@No78Vino
# Commite Date:2023.11.06
# DCC：Houdini 19.5 
# Level: Intermediate

参考了simon的教程：https://www.sidefx.com/tutorials/project-titan-gpt-signage/

商店标语立牌生成器。

在Simon版本的基础上加入了个人理解和修改，我不喜欢文字贴花部分再分一张纹理做渲染，浪费资源。
Simon的做法优势在于可以实现所有模型共用一个材质，如果真说资源节省Simon的做法确实更省。
但是这么做只针对uv展开简单且固定的模型，泛用性很低。而且他的normal纹理是被唯一的纹理限制死的。
我觉得这个做法有点太偏trick了，硬说trick应该也有别的更合适的手段。

## 使用方法
附带了shop.json文件，把这个json文件路径填入Board Info Json File的参数里即可。
剩余参数都比较好理解。

## 关于hda的贴花实现
我目前没有比较好的手段，用的方法是：贴画内容转模型，然后uv布局对应到要贴花的部位。

