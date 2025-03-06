# TS Server Module Help

This guide will help you set up tsserver in your JavaScript project.


## Step 1: Create jsconfig.json

Create jsconfig.json file in the root directory of your project

## Step 2: Enable "checkJs" in jsconfig.json

Since you’re not using TypeScript, create a jsconfig.json in your root directory to help tsserver handle JavaScript better:

```json
{
  "compilerOptions": {
    "module": "NodeNext",
    "moduleResolution": "NodeNext",
    "allowJs": true,
    "checkJs": true
  }
}
```
