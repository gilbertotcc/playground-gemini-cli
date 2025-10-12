# Gemini CLI playground

This playground lets technicians practice and experiment with
[Gemini CLI](https://geminicli.com/).
It is based on the
[Gemini CLI Tutorial Series](https://medium.com/google-cloud/gemini-cli-tutorial-series-77da7d494718)
and adds useful features such as custom sample commands and advanced
configuration scenarios relevant to real-world use.

## Setup

To set up the project, install Gemini CLI using the official
[Quick Install](https://github.com/google-gemini/gemini-cli?tab=readme-ov-file#quick-install)
guide.

Furthermore, to take full advantage of AI and use configured MCP servers (see
file `settings.json` in the folder `.gemini`), you may need to configure the
following environment variables.
Gemini CLI supports reading `.env` files, and it is strongly recommended to use
them to define the following variables.

Create a `.env` file in the project root and define these variables.

* `GITHUB_PAT`. GitHub Personal Access Token to interact with the GitHub API.
  For more information on creating a token, please refer to the GitHub
  documentation on
  [Managing your personal access tokens](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).

## References

* [Gemini CLI GitHub](https://github.com/google-gemini/gemini-cli)
* [Gemini CLI Tutorial Series](https://medium.com/google-cloud/gemini-cli-tutorial-series-77da7d494718)
