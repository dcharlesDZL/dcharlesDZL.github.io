## Typora Linux 安装后报错

**解决方法：**

root用户下修改

`/usr/share/applications/typora.desktop`

修改Exec项，加上`--no-sandbox` 即可

```desktop
Exec=typora %U --no-sandbox
```

修改后保存重新添加dock栏或者注销一下用户。