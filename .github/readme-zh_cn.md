[English](readme.md) | 中文 | [日本語](readme-ja_jp.md) | [Русский](readme-ru_ru.md)

![image](https://github.com/SillyTavern/SillyTavern/assets/18619528/c2be4c3f-aada-4f64-87a3-ae35a68b61a4)

移动设备界面友好，多种人工智能服务或模型支持（KoboldAI/CPP, Horde, NovelAI, Ooba, OpenAI, OpenRouter, Claude, Scale），类似 Galgame 的 老 婆 模 式，Horde SD，文本系统语音生成，世界信息（Lorebooks），可定制的界面，自动翻译，和比你所需要的更多的 Prompt。附带扩展服务，支持文本绘画生成与语音生成和基于向量数据库 的聊天信息总结。

基于 TavernAI 1.2.8 的分叉版本

### 由 Cohee、RossAscends 和 SillyTavern 社区为您呈现

注意：我们创建了一个 [帮助文档](https://docs.sillytavern.app/) 网站来回答各类问题与帮助您开始使用。

### SillyTavern 或 TavernAI 是什么？

SillyTavern 是一个可以安装在电脑（和安卓手机）上的用户界面，让您可以与文本生成的人工智能互动，并与您或社区创建的角色聊天/玩角色扮演游戏。

SillyTavern 是 TavernAI 1.2.8 的一个分支，正在进行更积极地开发，并添加了许多重要功能。在这一点上，它可以被视为完全独立的程序。

### 分支

SillyTavern 采用双分支进行开发，以确保所有用户都能获得流畅的使用体验。

* release -🌟 **推荐给大多数用户。** 这是最稳定、最推荐的分支，只有在重大版本推送时才会更新。适合大多数用户使用。
* staging - ⚠️ **不建议随意使用。** 该分支拥有最新功能，但要谨慎，因为它随时可能崩溃。仅适用于高级用户和爱好者。

如果你不熟悉使用 Git 命令，或者不了解什么是分支，别担心！release 分支始终是您的首选。

### 除了 SillyTavern，我还需要什么？

SillyTavern 本身并无用处，因为它只是一个用户聊天界面。你必须接入一个能充当角色扮演的人工智能系统。支持的人工智能系统有多种：OpenAPI API (GPT)、KoboldAI（可在本地或 Google Colab 上运行）等。您可以在 [常见问题](https://docs.sillytavern.app/usage/faq/) 中阅读更多相关信息。

### 我需要一台性能强大的电脑来运行 SillyTavern 吗？

由于 SillyTavern 只是一个用户聊天界面，它对硬件性能的要求很低，可以在任何电脑上运行。需要强大性能的是人工智能系统。

### 移动设备支持

> 注意

> **此分叉可使用 Termux 在安卓手机上原生运行。请参考 ArroganceComplex#2659 编写的指南：**

<https://rentry.org/STAI-Termux>

## 有问题或建议？

### 我们现在有了 Discord 社区

获取支持，或分享喜爱的角色和 Prompt：

### [加入 Discord 社区](https://discord.gg/sillytavern)

***

直接与开发人员联系：

* Discord: cohee 或 rossascends
* Reddit：/u/RossAscends 或 /u/sillylossy
* [发布 GitHub 问题](https://github.com/SillyTavern/SillyTavern/issues)

## 此版本包括

* 经过大量修改的 TavernAI 1.2.8（超过 50% 的代码经过重写或优化）
* 根据自定义规则自动重新生成消息
* 群聊：多机器人房间，供角色与你或彼此交谈
* 聊天书签/分支（复制当前状态下的对话）
* 先进的 KoboldAI / TextGen 生成设置，包含大量社区预设
* 支持世界信息（Lorebooks）：创建丰富的传说
* 支持 Window AI 浏览器扩展（运行 Claude、GPT 4 等模型）：<https://windowai.io/>
* [Oobabooga's TextGen WebUI](https://github.com/oobabooga/text-generation-webui) API 连接
* 连接 [AI Horde](https://horde.koboldai.net/)
* Prompt 生成格式调整
* Webp 角色卡支持（PNG 仍是内部格式）

## 扩展

SillyTavern 支持扩展服务，一些额外的人工智能模块可通过 [SillyTavern Extras API](https://github.com/SillyTavern/SillyTavern-extras) 提供。

* 作者注释/角色偏见
* 角色情绪识别
* 聊天记录自动摘要
* 在聊天窗口发送图片，并由人工智能解释图片内容
* 文本图像生成（5 预设，以及 "自由模式"）
* 聊天信息的文字转语音（通过 ElevenLabs、Silero 或操作系统的语音生成）

扩展服务的完整功能介绍和使用教程，请参阅 [Docs](https://docs.sillytavern.app/)。

## 界面/CSS/性能，由 RossAscends 调整并优化

* 针对 iOS 系统优化了界面，并支持将快捷方式保存到主屏幕，在全屏模式下打开。
* 热键
  * 上 = 编辑聊天中的最后一条信息
  * Ctrl+P = 编辑聊天中最后一条用户信息
  * 左 = 向左滑动
  * 右 = 向右滑动（注意：当聊天窗口输入内容时，轻扫快捷键将被禁用）
  * Ctrl+左 = 查看本地存储的变量（在浏览器控制台窗口中）
  * 回车（选择聊天栏）= 向人工智能发送信息
  * Ctrl+Enter = 重新生成人工智能最后的回复

* 用户名更改和角色删除不再强制重新刷新页面。

* 增加在页面加载时自动连接 API 的选项。
* 增加选项，在页面加载时自动加载最近的聊天信息。
* 更好的 Tokens 计算器 - 适用于未保存的文字，并显示永久和临时 Tokens 数量

* 更好的聊天历史查询窗口
  * 聊天的文件名以"（角色卡名称）+（创建时间）"的可读格式保存
  * 聊天历史预览从 40 个字符增加到 300 个字符。
  * 聊天历史排序有多种选择（按名称、创建日期、聊天记录大小）。

* 默认情况下，左侧和右侧弹出的设置面板会在点击其他区域时自动关闭。
* 点击导航面板上的 "锁按钮" 将保持弹出面板打开，并在不同聊天中记住此设置。
* 导航面板的打开或关闭状态也会跨聊天保存。

* 自定义聊天界面：
  * 收到新消息时播放提示音
  * 切换圆形或长方形头像样式
  * 在台式电脑上拥有更宽的聊天窗口
  * 可选的半透明玻璃效果聊天窗口
  * 可定制 "主文本"、"引用文本 "和 "斜体文本 "的字体颜色。
  * 可定制聊天界面的背景颜色和透明模糊程度

## 安装

*注意：SillyTavern 用于本地安装，尚未在 Colab 或其他云服务上进行全面测试。

> **警告**

> 切勿安装到任何受 Windows 控制的系统文件夹（Program Files, System32, etc）中。

> 不要以管理员权限运行 start.bat

### Windows

通过 Git 安装（推荐使用，便于更新）

附有精美图片示例的简易指南：
<https://docs.sillytavern.app/installation/windows/>

  1. 安装 [NodeJS](https://nodejs.org/en)（建议使用最新的 LTS 版本）
  2. 安装 [GitHub 客户端](https://central.github.com/deployments/desktop/desktop/latest/win32)
  3. 打开 Windows 资源管理器 (`Win+E`)
  4. 浏览或创建一个不受 Windows 控制或监控的文件夹。(例如：C:\MySpecialFolder\)
  5. 点击顶部的 "地址栏"，在该文件夹内打开命令提示符，输入 `cmd`，然后按回车。
  6. 弹出黑框（CMD 命令提示符）后，键入以下其中一项并按 Enter：

* 稳定分支：`git clone https://github.com/SillyTavern/SillyTavern -b release`
* 开发分支： `git clone https://github.com/SillyTavern/SillyTavern -b staging`

  7. 等待 Git 克隆完成后，双击文件夹中的 `Start.bat` 将启动 NodeJS 并开始自动安装需要的软件包。
  8. 然后 SillyTavern 服务就会自动启动，同时在浏览器新标签页中自动打开。

通过压缩包下载安装（不推荐）

  1. 安装 [NodeJS](https://nodejs.org/en)（建议使用最新的 LTS 版本）
  2. 从该 GitHub 仓库下载压缩包。(从 [Releases](https://github.com/SillyTavern/SillyTavern/releases/latest) 获取 "Source code（zip）"）。
  3. 将压缩包解压到您选择的文件夹中
  4. 双击或在命令行中运行 `Start.bat`。
  5. SillyTavern 服务自动为你准备好一切后，会在你的浏览器中打开一个新标签页。

### Linux

  1.运行 `start.sh` 脚本。
  2.等待自动完成，然后开始享受

## API 密钥管理

SillyTavern 会将 API 密钥保存在目录中的 `secrets.json` 文件内。

默认情况下，输入密钥并重新加载页面后，密钥会自动隐藏以保证安全。

如果要想通过点击 API 输入框旁边的按钮来查看密钥，请按照以下设置：

1. 打开 `config.yaml` 文件，将里面的 `allowKeysExposure` 设置为 `true`。
2. 然后重启 SillyTavern 服务。

## 远程访问

这通常是为那些想在手机上使用 SillyTavern 的人准备的，而他们的电脑和手机在同一个局域网中。

不过，SillyTavern 也可以被设置为允许从任何地方进行远程访问。

**重要提示：SillyTavern 是单用户程序，因此任何人登录后都能看到所有的角色卡和聊天内容，并能更改任何设置。

### 1.管理白名单 IP

* 在你的 SillyTavern 文件夹中新建一个文本文件，名为 `whitelist.txt`。
* 用文本编辑器打开该文件，添加你希望允许连接的 IP 地址列表。
* 接受单个 IP 地址和 IP 范围，示例：

```
192.168.0.1
192.168.0.20
```

或者

```
192.168.0.*
```

(上述 IP 范围将允许局域网中的任何设备连接）

也接受子网掩码设置（如 10.0.0.0/24）。

* 保存`whitelist.txt`文件。
* 重启 SillyTavern 服务。

然后，文件中设置的 IP 就可以访问 SillyTavern 了。

*注意："config.yaml" 文件内也有一个 "whitelist" 设置，你可以用同样的方法设置它，但如果 "whitelist.txt" 文件存在，这个设置将被忽略。

### 2.获取 SillyTavern 服务的 IP 地址

白名单设置完成后，您需要 SillyTavern 服务的 IP 地址。

如果 SillyTavern 服务设备在同一个局域网上，则使用安装 SillyTavern 服务的电脑的局域网 IP 地址：

* Windows：Windows 按钮 > 在搜索栏中输入 `cmd.exe` > 在打开的控制台中输入 `ipconfig`，回车 > 然后在输出中查找 `IPv4` 地址。

如果您（或其他人）想在互联网中访问你自己的 SillyTavern 服务，则需要运行 SillyTavern 服务的设备的互联网 IP 地址。

* 使用运行 SillyTavern 的设备，访问 [this page](https://whatismyipaddress.com/) 并查找 `IPv4`。这是您从互联网访问时要用到的。

### 3. 使用其他设备访问 SillyTavern 服务

无论你最终使用的是什么 IP 地址，都要将该 IP 地址和端口号输入其他设备网络浏览器。

同一局域网中的 SillyTavern 服务的典型默认地址如下：

`http://192.168.0.5:8000`

使用 http:// 而不是 https://

### 向所有 IP 开放您的 SillyTavern 服务

我们不建议这样做，但您可以打开 `config.yaml` 并将里面的 `whitelistMode` 设置改为 `false`。

你必须删除（或重命名）SillyTavern 文件夹中的 `whitelist.txt` 文件（如果有的话）。

这通常是不安全的做法，所以我们要求在这样做时必须设置用户名和密码。

用户名和密码在`config.yaml`文件中设置。

重启 SillyTavern 服务后，只要知道用户名和密码，任何设备都可以访问。

### 还是无法访问？

* 为 `config.yaml` 文件中的端口创建一条入站/出站防火墙规则。切勿将此误认为是路由器上的端口转发，否则，有人可能会发现你的聊天隐私，那就大错特错了。
* 在 "设置" > "网络和 Internet" > "以太网" 中启用 "专用网络" 配置。这对 Windows 11 非常重要，否则即使添加了上述防火墙规则也无法连接。

### 性能问题？

尝试在用户设置面板上关闭模糊效果（快速用户界面）模式。

## 我喜欢你的项目！我该如何贡献自己的力量？

### 应该

1. 发送 Fork 请求
2. 使用规定的模板发送功能建议和问题报告
3. 在提出任何问题之前，请先阅读 Readme 文件和文档

#### 不应该

1. 提供金钱捐赠
2. 发送错误报告而不提供任何详细信息
3. 提出已经回答过无数次的问题

## 我在哪里可以找到以前的聊天背景图片？

我们正在实行 100% 原创内容的政策，因此旧的背景图片已从该资源库中删除。

不过你可以在这里找到它们的存档：

<https://files.catbox.moe/1xevnc.zip>

## 屏幕截图

<img width="400" alt="image" src="https://user-images.githubusercontent.com/18619528/228649245-8061c60f-63dc-488e-9325-f151b7a3ec2d.png">
<img width="400" alt="image" src="https://user-images.githubusercontent.com/18619528/228649856-fbdeef05-d727-4d5a-be80-266cbbc6b811.png">

## 许可证和贡献

**发布本程序是希望它能有所帮助，但不做任何保证；甚至没有明示的性能、稳定性和其他任何特定用途的可用性保证。更多详情，请参阅 GNU Affero 通用公共许可证。**

**This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.**

* TAI Base by Humi: Unknown license
* Cohee's modifications and derived code: AGPL v3
* RossAscends' additions: AGPL v3
* Portions of CncAnon's TavernAITurbo mod: Unknown license
* kingbri's various commits and suggestions (<https://github.com/bdashore3>)
* StefanDanielSchwarz's various commits and bug reports (<https://github.com/StefanDanielSchwarz>)
* Waifu mode inspired by the work of PepperTaco (<https://github.com/peppertaco/Tavern/>)
* Thanks Pygmalion University for being awesome testers and suggesting cool features!
* Thanks oobabooga for compiling presets for TextGen
* KoboldAI Presets from KAI Lite: <https://lite.koboldai.net/>
* Noto Sans font by Google (OFL license)
* Icon theme by Font Awesome <https://fontawesome.com> (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License)
* AI Horde client library by ZeldaFan0225: <https://github.com/ZeldaFan0225/ai_horde>
* Linux startup script by AlpinDale
* Thanks paniphons for providing a FAQ document
* 10K Discord Users Celebratory Background by @kallmeflocc
* Default content (characters and lore books) provided by @OtisAlejandro, @RossAscends and @kallmeflocc
* Korean translation by @doloroushyeonse
* 中文翻译由 [@XXpE3](https://github.com/XXpE3) 完成，中文 ISSUES 可以联系 @XXpE3
