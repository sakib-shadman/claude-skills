# galacticos-labs: Claude Code plugins

This repository is the **galacticos-labs** plugin marketplace for [Claude Code](https://code.claude.com). It's a catalog: each plugin lives and is versioned in its own repository, and this repository lists them so you can add them all with one command.

## Add the marketplace

In a Claude Code session:

```text
/plugin marketplace add sakib-shadman/claude-skills
```

Or from your shell:

```bash
claude plugin marketplace add sakib-shadman/claude-skills
```

Then browse the plugins with `/plugin` (**Discover** tab), or install one by name as shown below.

## Plugins

| Plugin | What it does | Install |
| :- | :- | :- |
| [bug-workflow](https://github.com/sakib-shadman/bug-workflow) | Investigates bugs read-only into an evidence-based report, then implements the approved fix behind explicit approval gates. Skills: `investigate-bug`, `fix-bug`. | `/plugin install bug-workflow@galacticos-labs` |

`/plugin install` opens the plugin's details. Choose **Install for you (user scope)** to use it in every project. From the shell, `claude plugin install bug-workflow@galacticos-labs` installs at user scope by default.

Each plugin's README covers usage, configuration, and limitations.

## Updates

Auto-update is off by default for third-party marketplaces. Either:

- turn it on: run `/plugin`, open **Marketplaces**, select `galacticos-labs`, and choose **Enable auto-update**; or
- update manually: run `/plugin marketplace update galacticos-labs` in a session, or `claude plugin update <plugin>@galacticos-labs` in your shell.

To remove the marketplace and every plugin installed from it:

```bash
claude plugin marketplace remove galacticos-labs
```

If you don't have a GitHub SSH key and adding the marketplace or installing fails, set `CLAUDE_CODE_PLUGIN_PREFER_HTTPS=1` and try again.

## Issues

Report problems with a plugin in that plugin's repository, for example [bug-workflow issues](https://github.com/sakib-shadman/bug-workflow/issues). Use this repository's issues only for problems with the catalog itself.

## License

[MIT](LICENSE)
