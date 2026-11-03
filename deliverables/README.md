# 三场地3D瑞雷波 Fortran 工程

## Visual Studio 工程版 v2（推荐）

下载 [rayleigh_visual_studio_v2.zip](rayleigh_visual_studio_v2.zip)，解压。

1. 场地一打开 `OPEN_SITE1.sln`；场地二、三打开 `OPEN_SITE2.sln`、`OPEN_SITE3.sln`。
2. 在 Visual Studio 工具栏选择 **Release / x64**。
3. 按 **Ctrl+F5** 编译并启动。无需 Python、命令行或 bat。

需要已有 Intel Fortran 的 Visual Studio 集成和 Intel MKL。默认完整计算1个频率点。需要2点或300点，修改对应 `SiteN/run_settings.nml` 的 `nfreq`；结果自动写入 `SiteN/runs/` 新目录。

**验证边界：** 项目文件静态检查、GNU编译、无参数自动路径/目录和单点/双点自由场测试通过。修复大数组线程栈问题后，完整流程的有界启动检查已进入原始积分阶段，但尚未完成K/delta单频点验证。当前机器没有Windows/Visual Studio，未实测Intel Windows构建。瑞雷波自由场是对原始缺失激励的试用性补全，并非已验证的最终研究结果。详见包内说明与日志。

SHA-256：`e907a3f2bfaffe7174669b542b2a9235b435ce92ab251088ad86c75605bde712`

## 早期命令行试运行版 v1

[rayleigh_3d_v1.zip](rayleigh_3d_v1.zip) 保留供此前用户查阅。Visual Studio用户请优先使用上面的v2工程包。
