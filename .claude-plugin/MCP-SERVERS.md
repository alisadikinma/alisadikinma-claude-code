# MCP Servers Included

This plugin includes 3 pre-configured MCP servers that enhance Claude Code's capabilities.

## Included Servers

### 1. **Context7** (`@upstash/context7-mcp`)

**Purpose**: Access up-to-date, version-specific documentation for any library

**Usage**: Just mention "use context7" in your prompt when you need current library documentation

**Benefits**:
- Always up-to-date docs
- Version-specific information
- Works with thousands of libraries
- No manual searching required

---

### 2. **Playwright** (`@playwright/mcp`)

**Purpose**: Browser automation and web testing

**Capabilities**:
- Navigate websites
- Take screenshots
- Interact with web elements
- Generate test code
- Access accessibility trees

**Use Cases**:
- E2E testing
- Web scraping
- Browser automation
- Visual testing

**Integration with QA Expert Agent**:

The `qa-expert` agent uses Playwright MCP as its **primary tool** for mandatory task verification:

```yaml
qa_verification_flow:
  1. Launch browser instance
  2. Navigate to application
  3. Test CRUD operations
  4. Check console for errors
  5. Test responsive viewports
  6. Capture screenshot evidence
  7. Generate QA sign-off report
```

---

### 3. **Supabase** (`@supabase/mcp-server-supabase`)

**Purpose**: Supabase database operations

**Capabilities**:
- Query databases
- Manage tables
- Execute SQL
- Handle authentication
- Work with storage

**Use Cases**:
- Database management
- Schema exploration
- Data queries
- Admin operations

---

## Servers Not Included (Not Yet Available)

The following servers don't have official MCP implementations yet:

| Server | Status | Alternative |
|--------|--------|-------------|
| chrome-devtools | No official MCP | Use Playwright |
| stripe | No official MCP | Manual API |
| vercel | No official MCP | Vercel CLI |

---

## Using MCP Servers

After installing this plugin:

1. **Automatic Activation**: MCP servers start automatically when needed
2. **Restart Required**: Restart Claude Code after plugin installation
3. **Tool Access**: MCP tools appear in Claude's available tools list

---

## Agent-MCP Integration

| Agent | Primary MCP | Usage |
|-------|-------------|-------|
| `qa-expert` | Playwright | Browser testing, CRUD verification |
| `frontend-developer` | Playwright, Context7 | E2E tests, framework docs |
| `frontend-architect` | Context7 | Architecture patterns research |
| `backend-architect` | Supabase | Database schema design |
| `deep-research-agent` | Context7 | Technical documentation lookup |
| `performance-engineer` | Playwright | Performance testing |

---

## Adding More MCP Servers

Add custom MCP servers to your local `.claude/.mcp.json`:

```json
{
  "server-name": {
    "command": "npx",
    "args": ["-y", "package-name"],
    "env": {
      "API_KEY": "your-key"
    }
  }
}
```

---

## Troubleshooting

### MCP servers not loading?
1. Restart Claude Code
2. Check that npm/npx is installed
3. Verify network connection (MCP servers download on first use)

### Performance issues?
- MCP servers run on-demand
- First use may be slower (package download)
- Subsequent uses are fast

---

## Learn More

- Official MCP Documentation: https://modelcontextprotocol.io
- Claude Code MCP Guide: https://docs.claude.com/en/docs/claude-code/mcp
- MCP Server Directory: https://mcpcat.io
