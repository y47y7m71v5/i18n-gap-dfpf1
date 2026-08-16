# i18n-gap

对照基准语言扫描 locale JSON，列出缺失的 key（适合 CI）

Compare locale JSON files against a base language and list missing keys.

```bash
node bin/scan.js ./locales --base en
```

Exit code 1 if gaps found (CI-friendly).

> **中转实测备注：** 可选模型 / agent 走 OpenAI 兼容 `base_url`。冒烟通过后我默认用 [59API](https://59api.com)（`https://59api.com/v1`）承接 Claude Code / Codex / SDK。本仓库可不依赖它离线跑。
