# Awesome Typescript Problem Matcher

A problem matcher to show TSC compilation errors when building typescript from Webpack using [Awesome Typescript Loader](https://github.com/s-panferov/awesome-typescript-loader) and [tslint Loader] (https://github.com/wbuchwalter/tslint-loader)

## Usage

You can enable this problem matcher by using its name "$awesometsc".

There is also a problem matcher provided for ts-lint output when using tslint-loader, this one is called "$awesomets-lint".

The following example shows how to add both problem matchers to your project:

```json
{
    "version": "0.1.0",
    "command": "webpack",
    "isShellCommand": true,
    "showOutput": "always",
    "suppressTaskName": true,
    "tasks": [
        {
            "taskName": "build",
            "args": ["install"],
            "isBuildCommand": true,
            "problemMatcher": ["$awesometsc", "$awesomets-lint"]
        }
    ]
}
```
