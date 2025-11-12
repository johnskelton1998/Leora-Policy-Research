# Claude Code - Available Capabilities
**System Environment Documentation**

**Generated:** November 12, 2025
**User:** john@integritystudio.ai
**Organization:** Integritystudio

---

## 📦 Repository Information

**Current Repository:** Leora-Policy-Research
- **Location:** `/Users/johnskelton/Leora-Policy-Research`
- **Git Remote:** git@github.com:johnskelton1998/Leora-Policy-Research.git
- **Has .claude Config:** ❌ No (using global settings)
- **MCP Servers Enabled:** ✅ GitHub MCP (project-level)

---

## 🛠️ Built-in Tools

Claude Code has access to the following native tools in this environment:

### File Operations
| Tool | Description | Permission Status |
|------|-------------|-------------------|
| **Read** | Read file contents, supports images, PDFs, Jupyter notebooks | ✅ Always allowed |
| **Write** | Create new files | ✅ Always allowed |
| **Edit** | Modify existing files with exact string replacement | ✅ Always allowed |
| **Glob** | Pattern-based file searching (e.g., `**/*.js`) | ✅ Always allowed |
| **Grep** | Content search using ripgrep with regex support | ✅ Always allowed |

### Code Operations
| Tool | Description | Permission Status |
|------|-------------|-------------------|
| **NotebookEdit** | Edit Jupyter notebook cells | ✅ Always allowed |

### System Operations
| Tool | Description | Permission Status |
|------|-------------|-------------------|
| **Bash** | Execute shell commands (with timeout & sandboxing) | ⚠️ Selective permissions |
| **BashOutput** | Retrieve output from background bash processes | ✅ Always allowed |
| **KillShell** | Terminate background bash shells | ✅ Always allowed |

### Agent Operations
| Tool | Description | Permission Status |
|------|-------------|-------------------|
| **Task** | Launch specialized sub-agents for complex tasks | ✅ Always allowed |

### Planning & Mode Operations
| Tool | Description | Permission Status |
|------|-------------|-------------------|
| **ExitPlanMode** | Exit planning mode and proceed to execution | ✅ Always allowed |
| **TodoWrite** | Create and manage task lists | ✅ Always allowed |

### Information Gathering
| Tool | Description | Permission Status |
|------|-------------|-------------------|
| **WebSearch** | Search the web for current information | ✅ Always allowed |
| **WebFetch** | Fetch and analyze web page content | ⚠️ Domain restrictions apply |

### User Interaction
| Tool | Description | Permission Status |
|------|-------------|-------------------|
| **AskUserQuestion** | Ask user multiple-choice or open-ended questions | ✅ Always allowed |
| **Skill** | Execute installed skills from marketplaces | ✅ Always allowed |
| **SlashCommand** | Execute custom slash commands | ✅ Always allowed |

---

## 🤖 Sub-Agents

Claude Code can launch specialized sub-agents for specific tasks:

### Available Agent Types

| Agent | Purpose | Tools Available | When to Use |
|-------|---------|----------------|-------------|
| **general-purpose** | Complex multi-step tasks, code search, research | All tools (*) | Multi-step tasks requiring diverse capabilities |
| **Explore** | Fast codebase exploration | Glob, Grep, Read, Bash | Finding files by patterns, searching code keywords, answering codebase questions |
| **Plan** | Planning and exploration | Glob, Grep, Read, Bash | Same as Explore (fast planning agent) |
| **statusline-setup** | Configure status line settings | Read, Edit | Configuring Claude Code status line |
| **output-style-setup** | Create output styles | Read, Write, Edit, Glob, Grep | Creating Claude Code output styles |

### Agent Performance Tips
- Launch multiple agents concurrently when possible (use single message with multiple tool calls)
- Specify thoroughness level for Explore/Plan agents: "quick", "medium", or "very thorough"
- Agents are stateless - cannot send additional messages after launch

---

## 🔌 MCP Servers (Model Context Protocol)

### Currently Configured MCP Servers

#### GitHub MCP ✅ ENABLED
**Scope:** Project-level (home directory)
**Type:** stdio
**Command:** `npx -y @modelcontextprotocol/server-github`

**Environment Variables:**
```bash
GITHUB_PERSONAL_ACCESS_TOKEN=github_pat_11BZC6WHQ0GniboX84HMQ9_***
```

**Capabilities:**
- Create/update files in GitHub repositories
- Search repositories
- Create repositories
- Get file contents
- Push multiple files in single commit
- Create/manage issues
- Create/manage pull requests
- Fork repositories
- Create branches
- List commits
- Search code, issues, users
- Manage pull request reviews and merges

**Available GitHub MCP Tools:**
- `mcp__github__create_or_update_file`
- `mcp__github__search_repositories`
- `mcp__github__create_repository`
- `mcp__github__get_file_contents`
- `mcp__github__push_files`
- `mcp__github__create_issue`
- `mcp__github__create_pull_request`
- `mcp__github__fork_repository`
- `mcp__github__create_branch`
- `mcp__github__list_commits`
- `mcp__github__list_issues`
- `mcp__github__update_issue`
- `mcp__github__add_issue_comment`
- `mcp__github__search_code`
- `mcp__github__search_issues`
- `mcp__github__search_users`
- `mcp__github__get_issue`
- `mcp__github__get_pull_request`
- `mcp__github__list_pull_requests`
- `mcp__github__create_pull_request_review`
- `mcp__github__merge_pull_request`
- `mcp__github__get_pull_request_files`
- `mcp__github__get_pull_request_status`
- `mcp__github__update_pull_request_branch`
- `mcp__github__get_pull_request_comments`
- `mcp__github__get_pull_request_reviews`

**Permission Status:** ✅ Pre-approved in settings

---

## 🎨 Skills (Claude Skills Marketplace)

### Installed Marketplaces

#### awesome-claude-skills (ComposioHQ)
**Source:** https://github.com/ComposioHQ/awesome-claude-skills
**Last Updated:** November 5, 2025
**Location:** `/Users/johnskelton/.claude/plugins/marketplaces/awesome-claude-skills`

### Available Skills (26 total)

#### ✅ Enabled Skills (2)

| Skill | Description | Status |
|-------|-------------|--------|
| **lead-research-assistant** | Research assistant for lead generation and information gathering | ✅ Enabled |
| **content-research-writer** | Research and write comprehensive content | ✅ Enabled |

#### 📦 Available Skills (24)

| Skill | Category | Description |
|-------|----------|-------------|
| **algorithmic-art** | Creative | Generate algorithmic art patterns |
| **artifacts-builder** | Development | Build UI artifacts and components |
| **brand-guidelines** | Business | Create brand guideline documents |
| **canvas-design** | Creative | Design canvas layouts and mockups |
| **changelog-generator** | Development | Automatically generate changelogs from commits |
| **competitive-ads-extractor** | Marketing | Extract and analyze competitive advertisements |
| **document-skills** | Productivity | Document management and processing |
| **domain-name-brainstormer** | Business | Generate creative domain name ideas |
| **file-organizer** | Productivity | Organize files systematically |
| **image-enhancer** | Creative | Enhance and optimize images |
| **internal-comms** | Business | Create internal communications |
| **invoice-organizer** | Business | Organize and manage invoices |
| **mcp-builder** | Development | Build MCP server configurations |
| **meeting-insights-analyzer** | Business | Analyze meeting transcripts for insights |
| **raffle-winner-picker** | Utility | Pick random raffle winners |
| **skill-creator** | Development | Create new Claude Code skills |
| **slack-gif-creator** | Communication | Create GIFs for Slack |
| **template-skill** | Development | Template for creating new skills |
| **theme-factory** | Creative | Generate color themes |
| **video-downloader** | Utility | Download videos from URLs |
| **webapp-testing** | Development | Test web applications |

### How to Enable Skills

```bash
# Enable a skill
/plugin enable lead-research-assistant@awesome-claude-skills

# Disable a skill
/plugin disable lead-research-assistant@awesome-claude-skills

# List all skills
/plugin list
```

---

## 🔧 Plugins

### Plugin System Overview
Claude Code supports a plugin system that can extend functionality with:
- Custom slash commands
- Custom agents
- Hooks (pre/post tool execution)
- MCP servers

### Currently Installed Plugins
**Marketplace:** awesome-claude-skills
- 2 skills enabled (lead-research-assistant, content-research-writer)
- 24 skills available

### Plugin Commands

```bash
# Install a marketplace
/plugin install marketplace ComposioHQ/awesome-claude-skills

# Add a marketplace
/plugin marketplace add <github-repo>

# Enable/disable plugins
/plugin enable <plugin-name>
/plugin disable <plugin-name>

# Validate plugin configuration
/plugin validate

# List all plugins
/plugin list
```

---

## 🚀 Slash Commands

### Built-in Slash Commands

| Command | Description |
|---------|-------------|
| `/help` | Get help with Claude Code |
| `/agents` | Manage and view custom agents |
| `/permissions` | Manage tool permissions |
| `/mcp` | Manage MCP servers |
| `/plugin` | Manage plugins and skills |
| `/model` | Switch between models (Sonnet, Opus, Haiku) |
| `/config` | View/edit configuration settings |
| `/memory` | Manage memory files |
| `/todos` | View current todo list |
| `/cost` | View usage and costs |
| `/usage` | View plan limits |
| `/context` | Debug context issues |
| `/doctor` | Diagnose configuration issues |
| `/add-dir` | Add additional working directories |
| `/resume` | Resume previous conversations |
| `/rewind` | Undo code changes |
| `/clear` | Clear conversation history |
| `/export` | Export conversation |
| `/release-notes` | View release notes |
| `/upgrade` | Upgrade to Claude Max |
| `/status` | View system and account status |
| `/statusline` | Configure status line |
| `/terminal-setup` | Configure terminal settings |
| `/vim` | Enable vim mode |
| `/theme` | Change theme |

### Custom Slash Commands
**Location:** `.claude/commands/` directory

**This Repository:** ❌ No custom slash commands configured

**How to Create:**
1. Create `.claude/commands/` directory
2. Add markdown files (e.g., `mycommand.md`)
3. Files become slash commands (e.g., `/mycommand`)

---

## ⚙️ Permissions & Settings

### Current Permission Rules

**Allowed Tools:**
- None specifically pre-approved (uses default permissions)

**Denied Tools:**
- None

**Ask Before Use:**
- All tools require permission by default (except pre-approved ones)

**Pre-Approved MCP Servers:**
- ✅ github

### Global Settings
**Location:** `~/.claude/settings.json`

```json
{
  "permissions": {
    "allow": [
      "github"
    ],
    "deny": [],
    "ask": []
  },
  "enabledPlugins": {
    "lead-research-assistant@awesome-claude-skills": true,
    "content-research-writer@awesome-claude-skills": true
  }
}
```

### WebFetch Permissions
**Allowed Domains:**
- ✅ www.cmfgroup.com
- ✅ www.insureon.com

---

## 💾 Environment Details

### System Information
- **Platform:** macOS (Darwin 24.6.0)
- **Working Directory:** `/Users/johnskelton/Leora-Policy-Research`
- **Git Repository:** Yes
- **Shell:** bash
- **GitHub CLI:** Installed at `/opt/homebrew/bin/gh`
- **Git Protocol:** SSH (configured)

### Claude Code Configuration
- **Version:** 2.0.28 (latest)
- **Model:** Sonnet 4.5 (claude-sonnet-4-5-20250929)
- **Knowledge Cutoff:** January 2025
- **Account Type:** Claude subscription (Integritystudio organization)
- **Terminal Setup:** ✅ Configured (Option as Meta key enabled)

---

## 📊 Usage Statistics (Current Project)

**Last Session:**
- **Cost:** Not tracked yet (new project)
- **Web Searches:** 1 request
- **Tools Used:** Read, Write, Edit, Bash, WebSearch, WebFetch, TodoWrite
- **Files Created:** 3 (Safety_Program.md, Workers_Comp_Guide.md, README.md, Insurance_Comparison_CMF_vs_Insureon.md)

---

## 🎯 Quick Reference

### Most Useful Tools for This Repository

**Document Creation/Editing:**
- ✅ Read - Read existing policy documents
- ✅ Write - Create new documents
- ✅ Edit - Modify existing documents
- ✅ Grep - Search across all documents

**Research & Information:**
- ✅ WebSearch - Search for insurance/policy information
- ✅ WebFetch - Fetch specific insurance provider details
- ✅ lead-research-assistant (skill) - Research insurance companies
- ✅ content-research-writer (skill) - Write comprehensive documentation

**GitHub Operations:**
- ✅ All GitHub MCP tools - Manage this repository
- ✅ Bash (git commands) - Version control operations

**Planning & Organization:**
- ✅ TodoWrite - Track document creation tasks
- ✅ Task (Explore agent) - Explore large policy documents

---

## 💡 How to Use This Information

### To Enable More Features:

1. **Add More Skills:**
   ```bash
   /plugin enable <skill-name>@awesome-claude-skills
   ```

2. **Install More MCP Servers:**
   ```bash
   claude mcp add
   ```

3. **Create Custom Slash Commands:**
   - Create `.claude/commands/` in this repository
   - Add markdown files for custom commands

4. **Adjust Permissions:**
   ```bash
   /permissions add Bash(npm install:*)
   ```

### To See What's Available:
- `/help` - View all commands
- `/plugin list` - See all plugins/skills
- `/mcp` - View MCP servers
- `/agents` - View custom agents
- `/doctor` - Diagnose any issues

---

## 🔗 Additional Resources

### Documentation
- **Claude Code Docs:** https://docs.claude.com/en/docs/claude-code
- **MCP Documentation:** https://modelcontextprotocol.io
- **Plugin System:** https://docs.claude.com/en/docs/claude-code/plugins
- **Skills:** https://docs.claude.com/en/docs/claude-code/skills

### GitHub Resources
- **This Repository:** https://github.com/johnskelton1998/Leora-Policy-Research
- **Awesome Claude Skills:** https://github.com/ComposioHQ/awesome-claude-skills
- **Claude Code GitHub:** https://github.com/anthropics/claude-code

---

**Last Updated:** November 12, 2025
**Next Review:** When capabilities change or new features added

**Questions?** Use `/help` or `/doctor` for assistance.
