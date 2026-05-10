# 财税产品大师 部署速查卡

## 名称
财税产品大师

## 简介（填入平台「描述」字段）
面向深圳与香港企业服务场景，提供公司注册、工商变更、代理记账、审计报税、银行开户、注销及一次性业务的标准化咨询、报价、资料清单和办理指引。

## Token 信息
- 总量：约 15K tokens
- 建议模型：长上下文模型（上下文窗口 ≥ 16K）

## Monica 配置
- 主提示词：使用本地原始提示词全文，保持原文不改。
- Prompt Patch：将 `prompt_patch.txt` 追加到主提示词末尾。
- Skill Schema：将 `schema.json` 粘贴到 Monica 自定义技能的 OpenAPI Schema。
- 知识库来源：由 `schema.json` 指向本 GitHub 仓库的 raw 文件。

## 启动按钮（填入「会话开始示例」，最多4个）
1. 深圳注册内资公司需要哪些资料，多少钱？
2. 公司变更法人和地址分别怎么收费？
3. 一般纳税人代理记账一年多少钱？
4. 香港公司注册和年审怎么办理？

## 点击路径
Monica -> Bots / 自定义机器人 -> 选择财税产品大师 -> Skills / 自定义技能 -> 新增 OpenAPI Schema -> 粘贴 `schema.json` -> 保存；再回到 Bot Prompt 末尾追加 `prompt_patch.txt`。
