---
layout: post
title: Blockchain
subtitle: by twl
gh-repo: tianwenlong001/tianwenlong001.github.io
gh-badge: [star, fork, follow]
tags: [learning]
comments: true
---



solidity 智能合约  

web3j 封装 solidity   java  ethereum  

remix   truffle  



web3j 安装直接可以下载对应版本的bin包，然后配置环境变量即可使用

但是需要注意gradle  jdk对应的版本好，最好参考bin包对应源代码中的配置文件信息，选取对应的版本号才能够正常运行。

```sh
tap ethereum/ethereum
brew install ethereum
brew install ethereum --devel
brew update
brew upgrade
brew reinstall ethereum

docker pull ethereum/client-go
docker run -it -p 30303:30303 ethereum/client-go
docker stop ethereum/client-go
docker pull ethereum/client-go:latest
docker run -it -p 30303:30303 ethereum/client-go
```

编译部署合约可以通过solc，remix，truffle三个工具，最便捷的是使用remix，remix功能更加强大，但是remix产品化的同时也隐藏了很多实现细节，出问题不台容易排查，因此对于开发者来说，还是建议掌握solc和truffle命令来编译合约

https://docs.web3j.io/4.8.7/getting_started/run_node_locally/

https://www.javascript.com/learn/strings

https://ethereum.org/en/whitepaper/

https://github.com/Blockchain-zju/blockchainer-roadmap

https://trufflesuite.com/guides/nft-marketplace/



geth --sepolia --syncmode "light"  --discovery=true



https://www.geeksforgeeks.org/how-to-set-up-ganche-with-metamask/

metamask 

*sudo npm install -g ganache-cli*

**sudo npm install -g truffle**

进入工作目录

truffle init

撰写Contract， Migrate js, 还需要对truffle-config.js 进行修改，除了指定网络port 和network ID，还需要在该文件中指定降低solc编译的版本，0.8.13



针对编译后的contract生成Java wrapper

web3j generate truffle -t TestContract.json -o ./ -p com.contract

