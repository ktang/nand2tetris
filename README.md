# nand2tetris
From Nand to Tetris: Building a Modern Computer From First Principles

### Course materials
The official website for the Nand to Tetris course is [www.nand2tetris.org](https://www.nand2tetris.org/)
I've uploaded all the lecture and project description files to this repository for self-learning purpose. All the files can be downloaded at [www.nand2tetris.org/course](https://www.nand2tetris.org/course)

### Nand2Tetris Software Suite CLI install

I followed the this [instruction](https://github.com/nand2tetris/web-ide?tab=readme-ov-file#cli) to install the CLI tool but got error:
```{bash}
> npm install

npm ERR! code ENOTSUP
npm ERR! notsup Unsupported engine for @nand2tetris/web-ide@2025.36.0: wanted: {"node":">=16","npm":">=7"} (current: {"node":"14.15.4","npm":"6.14.10"})
npm ERR! notsup Not compatible with your version of node/npm: @nand2tetris/web-ide@2025.36.0
npm ERR! notsup Not compatible with your version of node/npm: @nand2tetris/web-ide@2025.36.0
npm ERR! notsup Required: {"node":">=16","npm":">=7"}
npm ERR! notsup Actual:   {"npm":"6.14.10","node":"14.15.4"}

npm ERR! A complete log of this run can be found in:
npm ERR!     ~/Users/akai~/.npm/_logs/2025-10-05T19_36_22_285Z-debug.log
```
So I need to update npm and node as follows:
#### update npm and node
```{bash}
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash

nvm install node       # installs latest Node.js + npm
nvm use node           # switch to latest
nvm alias default node # make it default version
```