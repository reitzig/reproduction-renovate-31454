# \#31454

Reproduced with GitHub application

## Current behavior

```
DEBUG: Datasource unknown error
{
  "datasource": "git-tags"
  "packageName": "git+https://github.com/copier-org/autopretty.git"
  "err": {
    "task": {
      "commands": [
        "ls-remote",
        "git+https://github.com/copier-org/autopretty.git"
      ],
      "format": "utf-8",
      "parser": "[function]"
    },
    "message": "git: 'remote-git+https' is not a git command. See 'git --help'.\n",
    "stack": "Error: git: 'remote-git+https' is not a git command. See 'git --help'.\n\n    at Object.action (/usr/local/renovate/node_modules/.pnpm/simple-git@3.26.0/node_modules/simple-git/src/lib/plugins/error-detection.plugin.ts:42:29)\n    at PluginStore.exec (/usr/local/renovate/node_modules/.pnpm/simple-git@3.26.0/node_modules/simple-git/src/lib/plugins/plugin-store.ts:54:29)\n    at /usr/local/renovate/node_modules/.pnpm/simple-git@3.26.0/node_modules/simple-git/src/lib/runners/git-executor-chain.ts:124:42\n    at new Promise (<anonymous>)\n    at GitExecutorChain.handleTaskData (/usr/local/renovate/node_modules/.pnpm/simple-git@3.26.0/node_modules/simple-git/src/lib/runners/git-executor-chain.ts:121:14)\n    at GitExecutorChain.<anonymous> (/usr/local/renovate/node_modules/.pnpm/simple-git@3.26.0/node_modules/simple-git/src/lib/runners/git-executor-chain.ts:97:40)\n    at Generator.next (<anonymous>)\n    at fulfilled (/usr/local/renovate/node_modules/.pnpm/simple-git@3.26.0/node_modules/simple-git/dist/cjs/index.js:52:24)"
  }
}
```

➡️ Job ID `0192042f-a796-7d51-b123-63b61252ce8a`


## Expected behavior

Renovate successfully looks up available versions of [copier-org/autopretty](https://github.com/copier-org/autopretty).

## Link to the Renovate issue or Discussion

[renovatebot/renovate#31454](https://github.com/renovatebot/renovate/discussions/31454)
