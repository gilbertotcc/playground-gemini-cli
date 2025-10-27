# Gemini CLI playground

This playground lets technicians practice and experiment with
[Gemini CLI](https://geminicli.com/).
It is based on the
[Gemini CLI Tutorial Series](https://medium.com/google-cloud/gemini-cli-tutorial-series-77da7d494718)
and adds useful features including custom sample commands and advanced
configuration scenarios relevant to real-world use.

## Setup

To set up the project, install Gemini CLI using the official
[Quick Install](https://github.com/google-gemini/gemini-cli?tab=readme-ov-file#quick-install)
guide.

Furthermore, to take full advantage of AI and use configured MCP servers (see
the file `.gemini/settings.json`), you may need to set the following environment
variables.

(Gemini CLI supports `.env` files, and it is strongly recommended to use them to
define the following variables.)

Create a `.env` file in the project root and define these variables.

* `GITHUB_PAT`. GitHub Personal Access Token to interact with the GitHub API.
  For more information on creating a token, please refer to the GitHub
  documentation on
  [Managing your personal access tokens](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).
* `GOOGLE_OAUTH_CLIENT_ID`, `GOOGLE_OAUTH_CLIENT_SECRET`. Google OAuth2
  credentials to interact with any Google API.
  For more information on creating these credentials, please refer to the
  [Google Cloud documentation](https://developers.google.com/workspace/guides/create-credentials).
* `OAUTHLIB_INSECURE_TRANSPORT`. This variable enables OAuthlib to work with
  HTTP callbacks, which is useful for local development.
  It is not recommended for production environments.
* `WORKSPACE_MCP_BASE_URI`, `WORKSPACE_MCP_PORT`. These variables are used to
  configure the Google Workspace MCP server.
  The base URI is the server address, and the port is the port number.
  For local usage, set `WORKSPACE_MCP_BASE_URI` to `http://localhost>` and
  `WORKSPACE_MCP_PORT` to `8000`.

## References

* [Gemini CLI GitHub](https://github.com/google-gemini/gemini-cli)
* [Gemini CLI Tutorial Series](https://medium.com/google-cloud/gemini-cli-tutorial-series-77da7d494718)

### MCP Servers

* [Getting started with the Atlassian Rovo MCP Server](https://support.atlassian.com/atlassian-rovo-mcp-server/docs/getting-started-with-the-atlassian-remote-mcp-server/)
* [GitHub MCP Server](https://github.com/github/github-mcp-server)
* [Google Workspace MCP Server](https://github.com/taylorwilsdon/google_workspace_mcp)
* [Notion MCP](https://developers.notion.com/docs/mcp)
