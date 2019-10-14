# Why does this repo exist?

The purpose of this repository is to explore and explain the apparently nondeterministic behavior of `npm install`. The demos use the latest version of `npm` at the time of writing, which is 6.11.3 (`node` version 12.12.0).

# Questions to explore:

## Does `npm install` update the `package-lock.json` when the `package.json` has not changed?

1. Publish version 0.0.1 of `npm-demo-package-1`
1. Add dependency on version ~0.0.1 of `npm-demo-package-1` in `npm-demo-client` and `npm install`
1. Publish version 0.0.2 of `npm-demo-package-1`
1. `npm install` in `npm-demo-client`

## What does deleting `node_modules` do?

## What does the `package-lock.json` actually do?

## Do transient dependencies get updated by `npm install` when those dependencies have new versions?