# Packages

This repository describes the process to create your own data visualizations for [RedisInsight](https://redis.com/redis-enterprise/redis-insight/) Workbench and provides the following quick and simple examples:

- [CLIENT LIST](https://github.com/RedisInsight/Packages/tree/main/clients-list-example) visualization
- [Random key](https://github.com/RedisInsight/Packages/tree/main/random-key-example) example



## Running locally

The following commands will install dependencies and start the server to run plugins locally:
```
yarn
yarn start
```
These commands will install dependencies and start the server. 

_Note_: Base styles are included to `index.html` 
from [RedisInsight](https://github.com/RedisInsight/RedisInsight) repository.

_From RedisInsight Repo_:
This command will generate the `vendor` folder with styles and fonts of the core app. Add this folder 
inside the folder for your plugin and include appropriate styles to the `index.html` file.

```
yarn build:statics - for Linux or MacOs
yarn build:statics:win - for Windows
```

## Build plugin

The following commands will build plugins to be used in RedisInsight:
```
yarn
yarn build
```

[Add](https://github.com/RedisInsight/RedisInsight/blob/main/docs/plugins/installation.md) the package.json file and the 
`dist` folder to the folder with your plugin, which should be located in the `plugins` folder.
