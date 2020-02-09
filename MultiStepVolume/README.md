# 多级音量

**解决问题**：听歌的时候感觉加一格音量太大，减一格音量太小

音量阶数越多，按一下音量上或音量下改变的音量越小，实现音量精细调节

通过`system.prop`(Magisk配置文件)向`build.prop`(系统配置文件)注入下面代码实现

```shell
#音量阶数，如果觉得30太多可以适当减小
ro.config.media_vol_steps = 30
#关闭大音量警告(如果调的音量过大会弹出的一个警告框)
audio.safemedia.bypass = true
```

**适用机型**：安卓机应该都通用；

实测红米 Note 4X(mido)，红米 K20 PRO(raphael)都可用

