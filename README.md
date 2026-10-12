# GTA Online · Angel 原声片段

这是从用户提供的《All AI Assistant Voicelines GTA Online A Safehouse in the Hills》音频中剪出的 Angel 语音片段，供已获相应使用许可的人检索和试听。仓库包含 52 段 MP3 压缩包、时间清单和制作说明。

## 文件

| 文件 | 内容 |
| --- | --- |
| [`MP3.7z`](MP3.7z) | 52 段 MP3，解压后位于 `MP3/` 文件夹。 |
| [`片段清单.csv`](片段清单.csv) | 文件名、原视频时间范围、时长、剪辑方式及来源链接。 |
| [`来源与下载状态.txt`](来源与下载状态.txt) | 原始来源、剪辑方法、音频参数和质量检查说明。 |
| [`SHA256SUMS.txt`](SHA256SUMS.txt) | 压缩包的 SHA-256 校验值。 |

## 来源与制作

- 游戏作品：**Grand Theft Auto Online — A Safehouse in the Hills**。
- 原视频：[All AI Assistant Voicelines GTA Online A Safehouse in the Hills](https://www.youtube.com/watch?v=s8q95G9dcC8)。上传者 **Lucas7yoshi**，据随附的本地来源说明记录；本仓库不是该视频或游戏的官方发布渠道。
- 使用的视频时间段：Angel 章节约 `00:00–15:32`；片段覆盖到 `15:27.767`。
- 从提供的 MP3 在低电平停顿处切分连续对白，保持原速，未变声、合成语音或添加音乐。每段约 15–20 秒。
- 压缩包内为 **44.1 kHz、单声道、192 kbps MP3**。原工作目录还生成过 WAV，但本仓库的压缩包**不包含 WAV**。

更具体的处理和检查结果见 [`来源与下载状态.txt`](来源与下载状态.txt)。

## 如何使用

1. 下载 [`MP3.7z`](MP3.7z)。用 [7-Zip](https://www.7-zip.org/) 解压，或在已安装 7-Zip 的终端运行：

   ```text
   7z x MP3.7z
   ```

2. 解压后的 `MP3/` 目录中，每个文件名对应清单的“文件名”列，再加 `.mp3` 后缀。例如 `Angel_01_15.98s` 对应 `MP3/Angel_01_15.98s.mp3`。
3. 用 [`片段清单.csv`](片段清单.csv) 查找片段在原视频里的开始、结束时间；使用前试听，确认对白边界和背景声音符合你的需求。
4. 如需核对下载完整性，可对 `MP3.7z` 计算 SHA-256，并与 [`SHA256SUMS.txt`](SHA256SUMS.txt) 比较。在 Windows PowerShell 中可运行：

   ```powershell
   (Get-FileHash .\MP3.7z -Algorithm SHA256).Hash
   ```

## 权利与使用提醒

音频内容源自 **Grand Theft Auto Online**，原视频亦属于其上传者的作品。标注来源不等于获得再分发、商用、改编或训练模型的许可。本仓库未对这些音频授予新的许可证；使用、再发布或用于其他项目之前，请自行确认取得所需授权并遵守适用条款。

这些片段未经逐段人工听审或人声分离，不能保证所有切点都是句末，也不能保证完全没有背景声。WAV 曾由原 MP3 解码生成，不能恢复有损压缩前的音质；本仓库仅提供 MP3 压缩包。
