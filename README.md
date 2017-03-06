###多渠道快速打包
>多渠道的快速打包目前发现两种 一种是美团的 另一种是packer-ng-plugin
>这两种方法都进行了尝试，首先速度上都是很快的
>但美团的方法 虽然都进行了相关设置 但脚本打的渠道包 在原生的android 7.0上会提示包已经损坏 在小米android6.0上是正常的 其他设备未知
>第二种 方法亲测可行 使用方法github上 官方写的 已足够相信 但有一个坑 未提 就是设置build.gradle中biuldType中release中加上
signingConfig signingConfigs.release 不然就会报错。对着官方demo才改成功 特意在此记下 防止遗忘
