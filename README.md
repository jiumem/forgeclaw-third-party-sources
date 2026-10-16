# ForgeClaw Windows 随包组件的对应源码

本归档对应 Git for Windows v2.55.0.windows.5（官方二进制归档 SHA-256：58fdf5679db11901697d2257cd076c8cdc49d64fe641b3e64ad158f1c5bf9b8d），用于 ForgeClaw Windows 0.3.0-beta.15 的 Bash 与 Git/OpenSSH 资源。

packages/ 包含实际保留程序与 DLL 所属 38 个二进制包的精确版本源码包。每个源码包保留上游 PKGBUILD、构建补丁及源码；index.json 记录组件版本、上游直接下载地址、实得大小和 SHA-256。源码包来自 Git for Windows 的版本索引与发布资产，以及 MSYS2 官方 source package 仓库；这些原始源码包的许可、版权和归属保持不变。

使用 tar 解开 .src.tar.gz 或 .src.tar.zst，在相应 Git for Windows SDK/MSYS2 构建环境中按包内 PKGBUILD 和安装依赖构建。Git for Windows 自有补丁和构建文件已包含在其精确版本源码包中。package-versions.txt 保留官方上游整体版本清单；本归档采用的实际子集以 index.json 与 inventory/ 中的文件清单为准。

ForgeClaw 的分拆仅裁选原始程序、私有依赖、许可证和配置；上游 EXE/DLL 字节保持原样。资源树内可直接阅读的包装脚本和配置随资源本体提供。完整上游构建方法见 https://gitforwindows.org/technical-overview.html ，源码包整理方法见 https://github.com/git-for-windows/build-extra/blob/main/get-sources.sh 。

校验：在归档根执行 shasum -a 256 -c SHA256SUMS.txt。各组件采用其上游原许可证，详见源码包内 COPYING、LICENSE、NOTICE 和 PKGBUILD。
