---
description: 演示在 Minecraft 客户端中使用 Yggdrasil
---

# 正版启动器

以下以 [Minecraft Launcher](https://www.minecraft.net/zh-hans/download) 为例，演示在 Minecraft 客户端中使用 Yggdrasil

{% hint style="success" %}
首先你得是正版，然后再皮肤站绑定正版，如发现进不去，可以去皮肤站的[个人资料](https://skin.vlssu.com/user/profile)右上角进行更新**UUID**
{% endhint %}

![](../../.gitbook/assets/h1b-b5usdthqh7-usdk9w_ol-1.png)

{% hint style="success" %}
需要先下载`authlib-injector.jar`[【点击下载】](https://authlib-injector.yushi.moe/~download/)并放在你的游戏文件的根目录也就是`.minecraft`文件夹里（实际随你放哪）
{% endhint %}

![](../../.gitbook/assets/fnuc00nk_mlxbxip03bgns.png)

{% hint style="warning" %}
然后打开正版启动器的JVM参数进行设置
{% endhint %}

{% tabs %}
{% tab title="设置参数" %}
这个参数中的`{绝对位置\authlib-injector.jar}`包括大括号一起替换成你的`authlib-injector.jar`绝对位置

```text
-javaagent:{绝对位置\authlib-injector.jar}=https://skin.vlssu.com/api/yggdrasil
```
{% endtab %}

{% tab title="这是我的参数" %}
这是我设置参数，仅供参考

```text
-javaagent:C:\Users\cmy13\AppData\Roaming\.minecraft\authlib-injector.jar=https://skin.vlssu.com/api/yggdrasil -Xmx8G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
```
{% endtab %}
{% endtabs %}

