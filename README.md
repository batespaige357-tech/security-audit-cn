# Security Audit CN

**用中文解释安全发现，用原始证据支撑结论。**

基于 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) 的小幅中文适配。独立社区版本，非官方。

## 上游能力保留

源码优先的防御性审查、guidance 与完整审计模式、六阶段工作流、信任边界、独立验证、隔离要求、结构化报告及覆盖检查。原正文和 19 份配套文件保留，包括 schema、校验器与其上游测试文件。

## 中文补充

- 已确认、待验证、已排除、未完成四种状态的中文解释，原 JSON 字段与枚举不改。
- 中文报告按主体、输入、边界、资源和证据说明具体发现。
- 保持原有隔离与验证门槛，不把语法检查包装成安全通过。
- 明确完整审计与局部咨询的范围，未完成的覆盖不称全面完成。

## 安装与调用

```bash
npx skills add batespaige357-tech/security-audit-cn --skill security-audit-cn
```

对助手说“用 security-audit-cn 只读审查这些文件，用中文报告证据和限制”；Codex 可输入 `$security-audit-cn`。也可复制 `skills/security-audit-cn` 整个目录到助手支持的技能目录，保留全部配套文件。

完整工作流需要适用的协作与 OS 隔离能力；报告校验器需要 Node.js。缺少执行控制时只做源代码分析并说明待验证内容。安装不自动执行目标代码、扫描线上服务或发送报告。没有示例网页、效果截图或前后对比。

## 来源与验证

MIT，保留 Cloudflare, Inc. 版权和完整许可。[CHANGES.md](CHANGES.md) 记录来源、改动和检查。

已检查正文与资源保留、UTF-8、本地链接、schema JSON 解析、技能格式及 JavaScript 语法。没有运行下载的校验器或测试文件，没有真实目标审计、漏洞验证或模型行为评估；不承诺发现率。未运行前端编译。
