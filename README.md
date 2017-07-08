# Awesome Typescript Problem Matcher

A problem matcher to show TSC compilation errors when building typescript from Webpack using [Awesome Typescript Loader](https://github.com/s-panferov/awesome-typescript-loader)

## Usage

You can enable this problem matcher by using its name "$awesometsc", as shown in the following task.json:

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
            "problemMatcher": "$awesometsc"
        }
    ]
}
```
