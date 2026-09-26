# 缺爱姐姐 · CG 图床（私有）

本仓库是「从小缺爱，只有我一人爱着的亲姐姐居然对我？？？」角色卡的 CG 图床。

## 目录

- `shenmengxi/` → 沈梦曦（18 张）
- `wangxuanbing/` → 王萱冰（20 张）
- `lixinwan/` → 李欣婉（18 张）

## 文件命名

`<数字ID>-<语义slug>.webp`，例如 `cg-07-bed-cowgirl-upright-swaying.webp`。

- **数字 ID**（`cg-07`）是给 AI 与正则用的调用键，短且稳定，世界书里只列 ID + 场景短语。
- **语义 slug** 是给人看的画面描述，由 `_tools/cg-catalog.mjs`（逐张人工审阅得出）决定。
- 两者都由脚本生成，**不要手改文件名**；改画面描述请改 `cg-catalog.mjs` 后重跑上传。

## 索引

`manifest.json` 是唯一索引，每张图含：`id` / `file` / `slug` / `tier` / `scene` / `tags`
/ `loc` / `pos` / `act` / `cloth` / `mood` / `cum` / `sha256`。
`_source.json` 记录每个 ID 对应的原始文件名，便于溯源。

`tier` 分档：`portrait` 日常立绘 · `intimate` 亲密暧昧 · `explicit` 露骨 · `special` 剧情。

## 酒馆侧

通过 `_tools/cg-upload.mjs`（上传+缓存）与 `_tools/cg-sync.mjs`（拉取）同步到
`SillyTavern/data/default-user/user/files/cg/`，前端只读本地缓存，**token 不进入前端**。

生成时间：2026-09-26T05:25:33.986Z
