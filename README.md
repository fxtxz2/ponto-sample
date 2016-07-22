[![bintray](https://img.shields.io/bintray/v/zyl/maven/android-volley-utils.svg)](https://bintray.com/zyl/maven/android-volley-utils/_latestVersion)
# ponto-sample
Android中的WebView混合开发，主要用于js与java之间的互相调用，方便js的编码习惯，参考[Wikia/ponto](https://github.com/Wikia/ponto)，但是这个已经停止更新了，主要修改了js调用java，能够有JSONOjbect对象返回给js。

# 修改部分
```java
#修改类为com.wikia.ponto.Ponto
// 添加native返回对象给js
responseParams = (JSONObject) method.invoke(object, params);
// 添加native返回对象给js
responseParams = (JSONObject) method.invoke(object);
```
# Gralde使用
```Gralde
compile 'com.wikia.ponto:ponto:0.0.1'
```
