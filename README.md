# 缺爱姐姐 · CG 图床（私有）

本仓库是「从小缺爱，只有我一人爱着的亲姐姐居然对我？？？」角色卡的 CG 图床。

## 目录

- `shenmengxi/` → 沈梦曦（18 张）
- `wangxuanbing/` → 王宣冰（20 张）
- `lixinwan/` → 李欣婉（18 张）

## 约定

- 图片统一 **WebP q85**，文件名 `cg-NN.webp`，由 `_tools/cg-upload.mjs` 生成，**不要手改**。
- `manifest.json` 是唯一索引：`tier`（portrait/intimate/explicit/special）、`tags`、`desc` 可人工补全，其余字段自动生成。
- `_source.json` 记录每个编号对应的原始文件名，便于溯源。
- 酒馆侧通过 `_tools/cg-sync.mjs` 拉取到本地缓存后读取，**token 不进入前端**。

生成时间：2026-09-26T05:12:15.360Z
