# IntelliJ IDEA 常用配置

## VM 参数修改

    Help > Edit Custom VM Options

通过调整 VM 参数来提升 IntelliJ IDEA 的运行速度。

- `-Xms128m` Xms是用来设置程序初始化时的内存大小，增加这个值的话程序的启动性能会得到提高，建议8G内存以上机器设置为：`-Xms512m`
- `-Xmx750m` Xmx是用来设置程序能够使用的最大内存数，如果程序要花很大内存的话，那就需要修改增加此数的值，建议8G内存以上机器设置为：`-Xmx1024m`
- `-XX:ReservedCodeCacheSize=240m` 缓存大小，建议8G内存以上机器设置为： `-XX:ReservedCodeCacheSize=512m`

## 主题字体修改

    File > Settings > Appearance & Behavior > Appearance

建议将主题设置为`Darcula`，字体设置为`Microsoft YaHei UI`，字号设置为`13`。

![3](./images/3.png)

## 文件编码设置

    File > Settings > Editor > File Encodings

![4](./images/4.png)

- 标注1所示，建议将`IDE Encoding`和`Project Encoding`设置为`UTF-8`。
- 标注2所示，IntelliJ IDEA 可以对`Properties`文件进行专门的编码设置，一般也建议改为`UTF-8`。
- 标注3所示，对于`Properties`文件，属性`Transparent native-to-ascii conversion`主要用于转换ASCII码，一般都要勾选，不然`Properties`文件中的注释显示的都不会是中文。
- 标注4所示，IntelliJ IDEA 除了支持对整个Project设置编码之外，还支持对目录、文件进行编码设置。如果你要对目录进行编码设置的话，可能会出现需要转换编码的弹出操作选择，强烈建议在转换之前做好文件备份，不然可能出现转换过程变成乱码，无法还原。
- 标注5所示，建议设置为UTF-8无BOM格式，即：`width NO BOM`。

## 显示工具栏、工具按钮

IntelliJ IDEA 默认是隐藏 `Toolbar` 和 `Tool Buttons` 的，如下图所示：

![1](./images/1.png)

可以通过如下菜单路径，进行开启：

    View -> Toolbar  
    View -> Tool Buttons

调整后的效果如下：

![2](./images/2.png)

## 参考资料

- [IntelliJ-IDEA-Tutorial](https://github.com/judasn/IntelliJ-IDEA-Tutorial)