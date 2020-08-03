# `@hchiam/deps` [![version](https://img.shields.io/npm/v/@hchiam/deps.svg?style=flat-square)](https://www.npmjs.com/package/@hchiam/deps) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/hchiam/deps/blob/master/LICENSE)

## Example usage:

This:

<img src="https://raw.githubusercontent.com/hchiam/deps/master/example.svg" height="300" title="The nodes are clickable, but only link to local files.">

was generated by this: (after you install [`@hchiam/deps`](https://www.npmjs.com/package/@hchiam/deps), not [`deps`](https://www.npmjs.com/package/deps))

```bash
deps
Enter max depth:
Enter src folder (or file or other folder you'd like to inspect): src
```

This interactive CLI tool `deps` generates a [dependency graph](https://en.wikipedia.org/wiki/Dependency_graph) of your files. You just have to give it a file or folder as a starting point. You can (optionally) tell it how deep to explore. It's basically a convenient but limited wrapper around [`depcruise`](https://www.npmjs.com/package/dependency-cruiser), which gives you an interactive SVG (clicking on nodes shows you code from local files).

## Install:

```bash
npm -g install @hchiam/deps
```

Now you can use it in any folder with this command:

```bash
deps
```

## Further development

Commands I found useful while creating the npm package for this CLI tool from scratch:

- `npm link`
- `rm /Users/howard/.nvm/versions/node/v10.13.0/bin/deps`
- `npm publish --access public`
