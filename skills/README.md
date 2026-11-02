# 可安装的 Codex Skills

## ai-dev-workflow

[查看 Skill](ai-dev-workflow/SKILL.md)：按需求、UI、技术方案、开发、验收和发布推进 AI 辅助软件开发。包含原规范、六份文档模板和项目 `AGENTS.md` 示例。

### 安装

需要 Git。以下命令将 Skill 安装到个人 `~/.agents/skills` 目录；已有同名目录时先检查并自行备份。

**Windows PowerShell**

```powershell
git clone --depth 1 https://github.com/lanke189/lanke189.git "$env:TEMP\lanke189-skills"
New-Item -ItemType Directory -Path "$HOME\.agents\skills" -Force | Out-Null
Copy-Item -LiteralPath "$env:TEMP\lanke189-skills\skills\ai-dev-workflow" -Destination "$HOME\.agents\skills\ai-dev-workflow" -Recurse
```

**macOS / Linux**

```bash
git clone --depth 1 https://github.com/lanke189/lanke189.git /tmp/lanke189-skills
mkdir -p ~/.agents/skills
cp -R /tmp/lanke189-skills/skills/ai-dev-workflow ~/.agents/skills/
```

安装后开启新的 Codex 会话，输入 `$ai-dev-workflow` 即可使用。
