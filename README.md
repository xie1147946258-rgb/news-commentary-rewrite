# 大鹏新闻短评改写 Skill

把新闻素材或已有评论改成直接、有态度、顺口的短评。核心要求：不复述新闻，短小精悍，金句戳痛点，联网参考热评；按本次要求决定犀利、强硬或中肯的程度。

当前版本：**1.0.0**（2026-11-27）。本仓库发布整理后的规则和示例，不包含原始聊天记录。

## 发给 Claude

把下面这段话和待改文案一起发给 Claude：

> 请先完整读取这个 Skill 的最新内容，再按里面的标准修改我接下来发来的新闻短评：
> https://raw.githubusercontent.com/xie1147946258-rgb/news-commentary-rewrite/main/SKILL.md
> 读取成功后告诉我读取到的版本。不要复述新闻，直接给一版可口播正文。如果链接无法读取，请明确告诉我，不要假装已经读取；我会上传 Skill 文件。

[查看 Skill 正文](./SKILL.md) · [查看版本变化](./CHANGELOG.md)

## 在 Claude 中安装

下载本仓库中的 `news-commentary-rewrite.zip`，上传到 Claude 的自定义 Skills 并启用。ZIP 内包含一个 `news-commentary-rewrite` 文件夹及其中的 `SKILL.md`。启用后，Claude 可在相关任务中按需选用；是否正确触发仍需用真实任务验证。

上传的 ZIP 是当时的版本。GitHub 上更新后，已上传的 ZIP 不会因此自动换新；可以重新上传新版，或在新对话中用上面的提示读取最新正文。仅发送 GitHub 链接，不等于已经安装 Skill。

官方使用说明：[创建、打包和启用自定义 Skills](https://support.claude.com/en/articles/12512198-how-to-create-custom-skills)。

## 维护方式

每日检查文件完整性、入口链接和已有的新反馈。发现具体问题或收到新的修改要求才更新；无新依据时保持当前版本。后续在 Claude 里的私人对话，需要你提供相关反馈后才能纳入更新。

示例验证场景见 [evals/cases.json](./evals.json)。文案的“爆款”效果不能通过格式校验保证，需结合真实发布效果迭代。
