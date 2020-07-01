# Typescript Solidity Dev Starter Kit


用于 Solidity智能合约开发的测试和部署的 Typescript 环境入门套件，使用[Buidler](https://buidler.dev)作为技术栈的平台层来协调所有任务。

使用[Ethers](https://learnblockchain.cn/docs/ethers.js/) 用于所有以太坊的交互和测试。

[博客文章](https://learnblockchain.cn/article/1196)


## 使用项目

克隆之后，用 `npm install` 安装依赖。
用  `npm run build` 构建， https://buidler.dev 有很棒的文档，可以用来扩展项目。


## 功能

### 编译及构建

`npm run compile`

### 生成TypeChain类型

`npm run build`

### 测试合约

`npm run test`

注意: 测试故意失败是为了演示Buidler的Solidity堆栈跟踪！

### 运行测试覆盖报告

`npm run coverage`

Note: The branch coverage is 75 %.

### 部署到Ethereum

创建/修改`buidler.config.ts`  中的网络，添加API key 和私钥，然后运行:

`npx buidler run --network rinkeby scripts/deploy.ts`

### Etherscan上验证代码

在 `buidler.config.ts` 加入 Etherscan API key，然后运行:

`npx buidler verify-contract --contract-name Counter --address <DEPLOYED ADDRESS>`

## 改进愿望

- 更好的迁移策略 (Buidler 已经在为此努力)


