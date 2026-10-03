# ⛔ 保护清单 —— 这些串绝对不能翻译

本文件后缀是 `.md` 不是 `.txt`，不会被当作词条加载。列在这里是给**人**看的。

## 图标查表键（译了图标就丢）

收集原文时容易混进这些，它们不是显示文字，是查图标的键
（对应 `Resources/` 下的图标资源）。译成中文 → 查不到图标 → 按钮变空白。

```
atom          chart-pie     chevron-right   chevron-down  clipboard-copy  close-x
copy-plus     category-plus dna             engine        eye
eye-dotted    floppy        focus-centered  folder        folder-symlink
histogram     keyframe      maximize        minimize      pencil-code
potion        settings      settings-cog    sort-ascending-shapes  square-half
square-rounded-x  sun       terminal        variable-plus  x-autolevel
x-drop        x-invert      x-macro         x-shaper      menu-deep
restore
```

> **注意大小写**：词典是大小写敏感的。上面这些图标键是小写；
> 而界面正常文本里出现的 `Histogram`（Match 节点的模式）、`Settings`（选项）、
> `Sun`（光照）是大写开头，**是显示文本，该译**。两者不冲突，别把图标键也译了。

## 文件格式标识（当扩展名/编码器用）

`PNG` `PNG8` `PNG16` `PNG64` `EXR` `TIFF8` `TIFF16` `TIFF32` `RAW` `R16`
`FloatRaw` `FloatRaw32` `HalfRaw` `HalfRaw16` `UshortRaw` `UshortRaw16` `GaeaRaw`
`OBJ` `FBX` `GLB` `GLTF` `DAE` `PLY` `PLY_BINARY` `CSV` `JPEG`

## 色彩空间标识符（下拉里照原样显示）

`CMY` `CMYK` `HCL` `HCLp` `HSB` `HSI` `HSV` `HWB` `Jzazbz` `LCH` `LCHab` `LCHuv`
`LMS` `Lab` `LinearGray` `Luv` `OHTA` `Oklab` `Oklch` `ProPhoto` `RGB` `sRGB` `scRGB`
`XYZ` `XyY` `YCC` `YCbCr` `YDbDr` `YIQ` `YPbPr` `YUV`

## 内部代码（不是给人看的）

- 单字母 `A`–`Z`、`Q 0` `Q 1`
- 卷积核代号：`C5X5B` `C5X5W` `C6X6B` `C6X6W` `C7X7B` `C7X7W` `H6X6A` `H6X6O` `H8X8A` `H8X8O` `O2X2` `O3X3` `O4X4` `O8X8` `HLINE` `DIAG`
- 数值尺寸：`_8` `_16` `_24` `_36` `_64` `_128` `_256` `_1024` `_2048`
- 疑似种子/哈希：`x4` `x16` `x127` `x253` `x505` `x513` `x1009` `x1025` `x2017` `x2049` `x4033` `x4097` `x8129` `x8193`
- 色彩空间：`BT601` `BT709`
- 泰森多边形变体：`VoronoiA` `VoronoiD` `VoronoiM` `VoronoiP` `VoronoiR` `VoronoiS`
- 距离函数：`Distance2Inv` `DistanceDiff` `DistanceInv` `DistanceToEdge`
- `LOD1`–`LOD6`、`V0` `V1` `V2` `X1` `X2` `X3` `X4` `X8` `XY` `XYZ`
- `minus2` `minus4` `plus2` `plus4` `zero`
- 文件/文件夹名、窗口标题里的工程名

> **例外：内置示例工程名已译**（60 个，在 `04_ui2.txt`）。它们同时也是
> `Examples\<名字>.terrain` 的实现文件名，但**实测安全**：译完点开一个示例，
> 图形/视口/属性面板全部正常加载 —— 说明 Gaea 是按背后的路径打开的，
> 不是拿显示文本去拼路径。侧作用是标题栏和「打开最近」也会显示中文名。
> 用户自己新建的工程名不要译（那会是真正的文件名，且用户会自己起名）。

## 品牌与产品名

`GAEA` `Gaea` `Unity` `Unreal` `Houdini` `Gaea2Unreal` `Gaea2Houdini`

> 右上角那串 `Gaea 2.3.0.1 Enterprise (Floating)` **已改译为「Gaea 2.3.0.1 企业版（浮动授权）」**
> （见 `04_ui2.txt`）。它原本列在这里，但拆开看只有版本号是产品名，
> `Enterprise` / `Floating` 是授权版本和授权方式，属于该说清的信息。
> 只改界面显示文字，不影响授权判定。Gaea 升级换版本号后要补新条目。
