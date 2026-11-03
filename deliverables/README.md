# 三场地3D瑞雷波0°试运行版 v1

下载本目录中的 `rayleigh_3d_v1.zip`，解压后先阅读“使用说明_先阅读.md”。

包含三个场地的 Fortran 源码、300点 CA 与频散输入、源码修改对照、编译运行脚本和实际测试日志。

Windows：在配置好 Intel oneAPI 与 Visual Studio 的命令行中执行：

```bat
build_windows.bat
run_windows.bat 1 1
```

第二条表示场地一、先算1点。场地二、三将第一个数字改为2、3；点数可选2或300。

**验证范围：** 三场地单点和双点自由场检查已通过；完整 K/delta 单频点与300点计算尚未完成验证，Windows Intel 编译脚本尚未实测。瑞雷波输入按单位地表竖向位移归一化，是对原始源码缺失激励的试用性补全。请勿将此包当作已验证的最终计算结果。

SHA-256：`40b1a153ec7cc1d537f046df51d843bdd8fa0fda2e2217b8efbe023f0a8e8f1a`
