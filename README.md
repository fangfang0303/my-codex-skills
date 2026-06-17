# personal-knowledge-ops

一个用于管理个人知识、个人技能、个人区域信息、外部领域内容和副业项目的 Codex skill。

## 安装方式

把这个仓库上传到 GitHub 后，其他人可以在 Codex 会话里直接说：

```text
帮我安装这个skill：https://github.com/fangfang0303/my-codex-skills/tree/main/personal-knowledge-ops
```

安装完成后，重开 Codex 或开启一个新会话即可生效。

## 使用方式

首次使用：

```text
@personal-knowledge-ops sync 初始化我的个人知识运营系统
```

日常使用：

```text
@personal-knowledge-ops sync
```

也可以在后面补充信息：

```text
@personal-knowledge-ops sync 我新增了一个技能：可以做健身新手训练计划
@personal-knowledge-ops sync 我这周测试了一个副业项目，有2个咨询
@personal-knowledge-ops sync 我新增了几个知识文件，顺便扫一遍外部机会
```

## 仓库结构

```text
personal-knowledge-ops-repo/
├─ README.md
└─ personal-knowledge-ops/
   ├─ SKILL.md
   ├─ README.md
   └─ EXAMPLE-TREE.md
```

实际安装使用的是 `personal-knowledge-ops/` 这个目录。

## 版本管理

发布目录中已经包含：

- `VERSION.md`
- `CHANGELOG.md`
- `REPO-INFO.md`

建议你每次更新时：

1. 修改 `VERSION.md`
2. 追加 `CHANGELOG.md`
3. 保持 `REPO-INFO.md` 中的仓库地址和安装链接正确

这样后续用户运行 skill 时，就可以被提醒是否有新版本可更新。

## 对外安装链接格式

如果你的仓库名叫 `my-codex-skills`，GitHub 用户名叫 `yourname`，那么安装链接建议写成：

```text
https://github.com/yourname/my-codex-skills/tree/main/personal-knowledge-ops
```

## 发布步骤

1. 把这个目录上传到 GitHub
2. 确保 `personal-knowledge-ops/` 在仓库里可见
3. 把上面的 GitHub 目录链接发给别人
4. 对方在 Codex 里说“帮我安装这个skill：<链接>”

## 说明

当前最稳妥的远程安装来源是 GitHub 路径。

如果你想做成自定义网站链接安装，还需要额外做一层安装分发机制；这不属于 skill 本身，而属于安装器生态扩展。
