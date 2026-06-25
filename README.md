# logo-skills

`logo-skills` 是一個用於產出與維護 Logo 設計交付標準的 Codex / agent skill package。此套件提供繁體中文 Logo 交付 SOP、交付檢查表、命名規則、資料夾結構、README 範本與版本管理規範，適合設計師、品牌顧問、外包廠商與企業內部專案管理人員使用。

## 目的

本 repository 的目標是將 Logo 設計交付流程標準化，確保 Logo 完成後可被穩定應用於：

- 官方網站與網頁介面
- App、PWA 與系統圖示
- 印刷品、包裝、招牌與特殊製程
- 簡報、提案、內部文件與品牌文件
- 社群媒體頭像、封面與行銷素材
- 品牌識別規範、設計系統與外部供應商交付包

## Repository 結構

```text
logo-skills/
├── SKILL.md
├── skill.json
├── LOGO_DELIVERY_STANDARD.md
├── references/
│   └── logo-delivery-standard.md
└── README.md
```

| 路徑 | 說明 |
|---|---|
| `SKILL.md` | Skill 的主要入口文件，包含使用情境、工作流程與輸出要求。 |
| `skill.json` | Skill package metadata，包含名稱、版本、入口點、授權、關鍵字、能力與更新策略。 |
| `LOGO_DELIVERY_STANDARD.md` | 可直接放入 Git repository 或公司知識庫使用的完整 Logo 設計交付標準文件。 |
| `references/logo-delivery-standard.md` | 供 skill 依 progressive disclosure 方式載入的完整 Logo 交付標準參考文件。 |
| `README.md` | 本 repository 的說明文件。 |

## Skill 資訊

| 欄位 | 內容 |
|---|---|
| Skill name | `logo-skills` |
| Version | `0.1.0` |
| Entry point | `SKILL.md` |
| Language | 繁體中文為主 |
| License | MIT |
| Primary reference | `references/logo-delivery-standard.md` |

## 適用情境

當使用者需要下列任一類型文件或規範時，可使用此 skill：

- Logo 設計交付標準 SOP
- Logo 交付項目清單
- Logo 檔案命名規則
- Logo 交付資料夾結構
- Logo 驗收檢查表
- Logo 使用規範與禁止使用範例
- 品牌色彩與字體交付規範
- Logo 設計 prompt 建議與 AI 概念發想範本
- favicon、App icon、社群頭像交付要求
- 品牌顧問或外包設計廠商交付規範
- 公司內部品牌資產管理文件

## 使用方式

### 1. 作為 Skill Package 使用

確認 repository 根目錄包含：

- `SKILL.md`
- `skill.json`
- `references/logo-delivery-standard.md`

使用 agent 或支援 skill package 的工具時，應以 `SKILL.md` 作為入口，並在需要完整 Logo 交付標準時讀取 `references/logo-delivery-standard.md`。

### 2. 作為公司 SOP 文件使用

若只需導入公司知識庫或專案 repository，可直接使用：

```text
LOGO_DELIVERY_STANDARD.md
```

建議依公司品牌、設計流程或採購驗收流程調整下列內容：

- 品牌負責人與聯絡窗口
- Logo 最小尺寸
- 社群媒體平台尺寸
- 印刷色彩管理要求
- 字體授權政策
- 專案驗收流程
- 版本管理與歸檔規則

### 3. 作為外包交付規範使用

可將 `LOGO_DELIVERY_STANDARD.md` 附於設計合約、委外需求書、採購需求文件或專案 brief 中，作為廠商交付與驗收依據。

建議於專案啟動時明確告知廠商：

- 必交與選交項目
- 檔案格式與尺寸需求
- 命名規則
- 資料夾結構
- 驗收清單
- 版本交付與 changelog 規則

## 文件內容摘要

`LOGO_DELIVERY_STANDARD.md` 與 `references/logo-delivery-standard.md` 目前包含以下章節：

1. 文件目的
2. 適用範圍
3. Logo 交付清單
4. 檔案格式標準
5. Logo 版本標準
6. 尺寸與解析度標準
7. 色彩規範
8. 字體規範
9. Logo 使用規範
10. 檔案命名規則
11. 資料夾結構
12. 驗收標準
13. README 範本
14. 版本管理
15. Logo 設計 Prompt 建議
16. 附則

## PDF 輸出注意事項

若需要將 Logo 交付標準或品牌規範輸出為 PDF，應先確認中文字體已正確嵌入，並於目標平台與 PDF viewer 中測試不會出現亂碼、缺字、字距異常或列印問題。若無法確保中文 PDF 正確顯示，請改以英文內容輸出 PDF，以降低供應商、客戶或跨平台檢視時的交付風險；繁體中文內容可保留於 Markdown、Figma 或其他可編輯來源文件中。

## 維護原則

更新本 repository 時，請遵循下列原則：

1. `SKILL.md` 應保持精簡，聚焦於 agent 需要遵循的流程與輸出要求。
2. 較長的 SOP、範本或詳細規範應放在 `references/` 目錄。
3. `skill.json` 的 `name` 應與 `SKILL.md` frontmatter 的 `name` 保持一致。
4. 若更新 `LOGO_DELIVERY_STANDARD.md`，應同步評估是否更新 `references/logo-delivery-standard.md`。
5. 若涉及重大規範變更，應更新 `skill.json` 的版本號。
6. 所有 Markdown 文件應保持繁體中文、正式、清楚且可執行的語氣。

## 版本管理

本 repository 採用語意化版本概念管理 skill package：

| 版本類型 | 說明 | 範例 |
|---|---|---|
| Patch | 修正錯字、格式、連結或小幅文件表述 | `0.1.1` |
| Minor | 新增章節、範本、檢查表或相容性功能 | `0.2.0` |
| Major | 調整 skill 結構、破壞相容性或大幅改寫核心標準 | `1.0.0` |

Logo SOP 文件本身可依文件內的版本管理規則使用 `v1.0`、`v1.1`、`v2.0` 等方式標示交付版本。

## 驗證建議

提交變更前，建議至少執行下列檢查：

```bash
python - <<'PY'
import json
import re
from pathlib import Path

manifest = json.loads(Path('skill.json').read_text(encoding='utf-8'))
skill = Path('SKILL.md').read_text(encoding='utf-8')
frontmatter = skill.split('---', 2)[1]
name = None
for line in frontmatter.splitlines():
    if line.startswith('name:'):
        name = line.split(':', 1)[1].strip()

assert manifest['schema_version'] == '0.1.0'
assert manifest['entrypoint'] == 'SKILL.md'
assert manifest['name'] == name
assert re.match(r'^[a-z0-9](?:[a-z0-9-]{0,62}[a-z0-9])?$', name)
assert Path('references/logo-delivery-standard.md').exists()
print('skill package validation: ok')
PY
```

## 授權

本 repository 使用 MIT License。若將本文件導入公司內部流程，仍應依公司法務、品牌、採購與設計管理規範調整實際使用條款。
