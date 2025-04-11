# GittHub-MCP-Serverr

1.Install nodejs vesrion V22.14.0
https://nodejs.org/en/download
Verify Installation
node -v  # Should return v22.14.0

2.Install npm - Bundled with Node.js (no separate install needed).
Verify 
npm -v

& Update npm (if needed):
npm install -g npm@latest

3.Install Claude Desktop
https://claude.ai/download
Follow OS-specific setup instructions.

4.Configure Clude Desktop 
Open Claude Desktop and sign in.
Navigate to Settings > API/Integrations.
config.json

{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-github"
      ],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "<YOUR_TOKEN>"
      }
    }
  }
}

5.Create a Github Account
Create a GitHub account: https://github.com/signup

6.Create Organization & repos
Create an organization (for team projects).
Create a new repository for your MCP Server.

7.Generate GitHub Personal Access Token (PAT)
Go to: Settings > Developer Settings > Personal Access Tokens
Permissions: Select repo, admin:org, workflow (adjust as needed).
Copy the token (store securely; it won’t be shown again).

8.Update tocken with Claude config json file
Locate Claude’s config file (typically config.json).
Add your GitHub PAT:


9.If Claude Desktop integration fails:

Close the app completely (right-click its icon in the system tray/taskbar → Exit).
Reopen Claude Desktop and retry the integration.
Still stuck? Check the logs (Help > View Logs) for errors."


