# Numbersf/Action-Build 上游更新报告

- 上游仓库: [Numbersf/Action-Build](https://github.com/Numbersf/Action-Build)
- 上游分支: `SukiSU-Ultra`
- 当前上游 HEAD: `1d28ca0`
- 新增提交数: 3

## 影响构建框架的提交

- `1d28ca0` 2026-10-29 refactor(susfs): rename PatchFakePatches to SusfsCompat, split out SusfsContext
- `9133c0a` 2026-10-28 feat(patch): add context mode to restore missing trace/hooks includes
- `ee0479e` 2026-10-28 fakepatch: 为缺少 trace/hooks/blk.h 的 android14-6.1 源码补上下文（修复 namespace.c hunk 失败） (#298)

## 上游 Workflow 相关提交

- `1d28ca0` 2026-10-29 refactor(susfs): rename PatchFakePatches to SusfsCompat, split out SusfsContext
- `9133c0a` 2026-10-28 feat(patch): add context mode to restore missing trace/hooks includes

## 上游文件变化概览

```text
 .github/workflows/Build Kernel OnePlus.yml        | 1644 +++++++++++++++++++++
 scripts/{PatchFakePatches.kts => SusfsCompat.kts} |   73 +-
 scripts/SusfsContext.kts                          |  119 ++
 3 files changed, 1777 insertions(+), 59 deletions(-)
```

## 注意

本报告只用于检查上游变化，不会覆盖 GT5 的 BakaSU、MIUIX、MD3 等定制逻辑。
