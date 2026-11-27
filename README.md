# nn-skills-marketplace

A Claude Code plugin marketplace of skills for Nikolai Nobadi's public Swift packages and architecture references. Each skill lives in the repo it documents, so the API and its docs change together. The full list is in [`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json).

## Install

```
/plugin marketplace add nikolainobadi/nn-skills-marketplace
/plugin install <PluginName>@nn-skills-marketplace
```

## Migrating from `nn-swift-skills`

This marketplace used to be called `nn-swift-skills`. Claude Code keeps a marketplace's old name when it updates, so remove it and add it again:

```
/plugin marketplace remove nn-swift-skills
/plugin marketplace add nikolainobadi/nn-skills-marketplace
```

Removing the marketplace uninstalls its plugins. Reinstall the ones you use with `/plugin install <PluginName>@nn-skills-marketplace`, and change any `enabledPlugins` entries in `.claude/settings.json` from `<PluginName>@nn-swift-skills` to `<PluginName>@nn-skills-marketplace`.
