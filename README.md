# zhangben-profile

Personal **plan / config pack** for [haytham-fu/zhangben](https://github.com/haytham-fu/zhangben) — **not** shipped with the public GitHub Pages site.

The live app at https://haytham-fu.github.io/zhangben/ is a **generic ledger**. This repo holds Haytham’s private-ish budget plan (3500+1500, daily plan, Sept 2026 opening summary + daily txs) so it can be loaded on demand.

## Files

| File | Purpose |
|------|---------|
| `haytham-ledger-profile.json` | Settings overlay + optional `transactions` (`version` + `settings` + `transactions`) |

## How to load in the app

1. Open **账本** → **设置** → **导入个人计划配置**
2. Choose one:
   - **从文件导入** — download this JSON and pick it
   - **从链接导入** — paste the raw URL below
   - **粘贴 JSON** — paste file contents

Import **merges settings + `monthOpening`**, and **merges `transactions` by id** (skips duplicates). Existing local txs are kept.

### Raw URL (after push to `main`)

```
https://raw.githubusercontent.com/haytham-fu/zhangben-profile/main/haytham-ledger-profile.json
```

Repo: https://github.com/haytham-fu/zhangben-profile

## What’s inside

- Monthly budget **5000** = **3500** basic + **1500** special  
- Daily plan compare amounts (Mon–Sun / Sat play|stay)  
- Fixed HKD **0.86** and preferred currencies RMB/HKD/USD/EUR  
- `monthOpening` for **2026-09** first-half summary (**9/1–9/15**, no daily line items)  
- `transactions` for **9/16–9/17** daily detail (calendar / day remain / monthly remain)  
- Octopus **topup** entries use `kind: "topup"` and **do not** count as budget spend

## Privacy

Keep this repo **private** if you prefer; the public zhangben site never bundles this file. A private raw URL still works when you’re logged into GitHub in the browser, or download the file and use「从文件导入」.
