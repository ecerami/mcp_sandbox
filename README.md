# mcp_sandbox
MCP Experiments

Code is forked and adapted from:  https://learn.deeplearning.ai/courses/mcp-build-rich-context-ai-apps-with-anthropic/lesson/dbabg/creating-an-mcp-server

To run the MCP Inspector:

```shell
npx @modelcontextprotocol/inspector uv run research_server.py
```

To run within Claude Desktop, modify yur `claude_desktop_config.json` like so.  Update the directory
to match your set-up.

```json
{
  "mcpServers": {
    "research_server": {
      "command": "/opt/homebrew/bin/uv",
      "args": [
        "--directory",
        "/Users/cerami/dev/mcp_sandbox",
        "run",
        "research_server.py"
      ]
    }
  }
}
```