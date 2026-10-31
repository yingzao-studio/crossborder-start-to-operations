## 豆包、DeepSeek与ChatGPT接入更新（2.1.3）

- ChatGPT原生技能：仅在账号具备Skills上传入口时使用目录包；官方规则已核对，未在你的账号安装或扫描。
- 普通聊天：使用[完整单文件](skill.txt)，或[启动提示词](chat/start.txt)；先验证模型确实读到所需正文。
- DeepSeek Harness：同名文件夹的SKILL.md入口与references，按官方的一层目录发现规则放置。
- 豆包原生技能导入：本次缺少官方格式和客户端实测依据，保留标准包候选，不标为已验证。
- [逐项官方核验、安装方式与未测范围](references/platform-compatibility.md)。文件存储、聊天参考和原生技能安装是不同能力。

<!-- PUBLIC-ACCESS:START -->
## 所有人可获取：DeepSeek · 豆包 · ChatGPT

**跨境从零开店与经营**

- [完整技能文本，复制后交给模型](https://raw.githubusercontent.com/yingzao-studio/crossborder-start-to-operations/main/%E9%80%9A%E7%94%A8%E6%8F%90%E7%A4%BA%E8%AF%8D.txt)
- [ZIP下载](https://github.com/yingzao-studio/crossborder-start-to-operations/releases/latest)
- [三平台使用步骤](三平台使用说明.md)

公开下载不代表官方目录收录；模型能否读附件、联网或自动读取链接取决于实际环境。
<!-- PUBLIC-ACCESS:END -->

# 跨境从零开店与经营 · v2.1.3

给还没开店、不知道卖什么的人使用：先问最多三个问题，从今天一项免费动作开始，再按条件推进选方向、算账、开店、上架、履约和复盘。

## 调用

使用 crossborder-start-to-operations。我还没开店，也不知道卖什么。先问最多三个问题，带我完成今天第一步；涉及政策、费用和数据，请联网核实并附来源，不要编造。

最少只需说清当前阶段；不知道的可以留空。默认不会要求你先填长问卷、购买软件或准备海外账户。

## 查看

- [技能入口](SKILL.md)
- [首轮交付演示](examples/first-session.md)
- [配置与使用](使用与跨模型配置.md)
- [更新与验证](更新与验证.md)

解压后将整个同名目录放入宿主技能目录，保留references。不支持技能目录时上传通用提示词.txt；具体联网、附件和操作能力由环境提供。普通聊天文本可用不代表所有模型已实测兼容。

演示不是客户成绩；流程不承诺开店获批、出单或盈利。没有数据就留未知。此版本已准备本地通用包，未提交官方插件目录。


## 标准、维护与许可

版本2.1.3。采用[MIT许可证](LICENSE)，第三方与历史素材的范围见[许可说明](THIRD_PARTY.md)。[本次官方规范核验](references/standards-review.md)列明来源与快照版本。
当前OpenAI文档列出的本地目录为~/.agents/skills及项目.agents/skills。旧版本或宿主可能有其他目录，按该工具实际技能列表确认，避免安装同名副本。此电脑已有的发现目录不在此次更新中迁移。
使用本技能无需安装Python依赖；维护校验才需要：先运行`python -m pip install -r requirements-dev.txt`，再运行`python -X utf8 scripts/validate_package.py`。GitHub检查配置已附带，但只有提交仓库并实际跑完后才可称CI通过。
[行为评估用例](evals/README.md)独立于文件校验，目前尚未完成独立模型实测。不把手写演示或结构通过称为成功案例。

## English quick start

Use the skill with your own source material. It produces a reviewable draft or a beginner's next action, keeps unknown facts explicit, and never assumes account access. Live research requires browsing; image production requires an image tool. Plain chat users can upload the bundled text instructions. Examples are synthetic, not customer results.

## 使用反馈

反馈时提供：使用的模型与工具、去敏后的最小输入、预期结果、实际结果及失败阶段。不要提交证件、凭据、买家信息或无权公开的截图。优先修复能复现的失败，再增加新功能；不以功能数量代替实用性。
