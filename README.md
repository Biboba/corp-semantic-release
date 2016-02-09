# corp-semantic-release - Work-in-progress.

Corporate semantic release for private projects under corporation network.

It contains all expected features by [semantic-release](https://github.com/semantic-release/semantic-release) but will not publish to **npmjs** at the end. 


## Actions performed

* detect if a release is required. If not, exit(0);
* figure out type of bump
* generate or append contents to `CHANGELOG.md` from last semantic tag
* bump your `package.json` only
* `git add package.json CHANGELOG.md` 
* `git commit -m "chore(build): release v1.0.0"`
* `git tag v1.0.0`
* `git push`
* `git push --tags`


## Install 
run: `npm install corp-semantic-release --save-dev`

## Configure


## Options
* `-d` or `--dryrun`: it runs in non-destructive mode. No alteration hsould be done in your workspace.
* `-v` or `--verbose`: it prints extra info such as commit list from last tag and command details.  

## Contribute
As usual, the same as [cz-customizable]()
