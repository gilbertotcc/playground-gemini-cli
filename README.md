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

Next, configure the following environment variables in a `.env` file.

* `GOOGLE_APPLICATION_CREDENTIALS`. Path to the service account JSON token used
  for sending logs and metrics to Google Cloud Platform.
* `GITHUB_PAT`. GitHub Personal Access Token to enable interaction with the
  GitHub API.
  For details on creating a token, refer to the GitHub documentation on
  [Managing your personal access tokens](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

## Observability

This project provides observability for the Gemini CLI by sending logs and
metrics to Google Cloud Platform.
To enable this, set the environment variable `GOOGLE_APPLICATION_CREDENTIALS` in
the `.env` file to your GCP service account JSON token.

The configuration follows the guidelines in
[Gemini CLI Tutorial Series : Part 13 : Gemini CLI Observability](https://medium.com/google-cloud/gemini-cli-tutorial-series-part-13-gemini-cli-observability-c410806bc112).
To disable observability, set `telemetry.enabled` to `false` in
`.gemini/settings.json`.

To test this feature locally, run the
[Docker OpenTelemetry LGTM](https://grafana.com/docs/opentelemetry/docker-lgtm/)
container and update the configuration to reference it.

## References

* [Gemini CLI GitHub](https://github.com/google-gemini/gemini-cli)
* [Gemini CLI Tutorial Series](https://medium.com/google-cloud/gemini-cli-tutorial-series-77da7d494718)

### MCP Servers

* [Getting started with the Atlassian Rovo MCP Server](https://support.atlassian.com/atlassian-rovo-mcp-server/docs/getting-started-with-the-atlassian-remote-mcp-server/)
* [GitHub MCP Server](https://github.com/github/github-mcp-server)
* [Notion MCP](https://developers.notion.com/docs/mcp)
