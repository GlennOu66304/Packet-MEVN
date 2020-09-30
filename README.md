## 1.first build the project set up:  
1.fetchMetadata: sill resolveWithNewModule caniuse-lite@1.0.30001008 checking issue fix  
1.Chinese Developer use:[npm换源](https://zhuanlan.zhihu.com/p/90561304)  
2.[npm install Error: rollbackFailedOptional](https://stackoverflow.com/questions/46011546/npm-install-error-rollbackfailedoptional)  
3.[What is the --save option for npm install?](https://stackoverflow.com/questions/19578796/what-is-the-save-option-for-npm-install) 

## 2.connect to database:
config fold needs to be under the server fold;  
[internal/modules/cjs/loader.js:582 throw err](https://stackoverflow.com/questions/53545800/internal-modules-cjs-loader-js582-throw-err#54964538)  

## 4. TypeError: Router.use() requires middleware function but got a Object and Webpack undefined 
1. You need to make sure that use the comma in the code below:  
```
v1Router.use('api/v1/auth', authRouter)  
```
2. all webpack issue in the terminal, you need to make sure that all webpack used the same version of"w" or "W".  

## 5. Issue fixing while you download the repository from the github:  
1. [nodemon not working: -bash: nodemon: command not found](https://stackoverflow.com/questions/35530930/nodemon-not-working-bash-nodemon-command-not-found)  
2. [https://stackoverflow.com/questions/35530930/nodemon-not-working-bash-nodemon-command-not-found](https://github.com/rwieruch/minimal-node-application/issues/new)  
3. URL to see the content in the browser:http://localhost:3000/  

## 6.Adding Vue loader to webpack:
1.[vue-loader v15 requires VueLoaderPlugin in webpack config #1453](https://github.com/rails/webpacker/issues/1453) 
solution:
```
const VueLoaderPlugin = require('vue-loader/lib/plugin')
...
plugins: [
  new VueLoaderPlugin()
]
``` 


## Resource List:  
1.Project Resource List:[Fullstack Enterprise MEVN: Mongo, Express, Vue, and Node](https://learning.oreilly.com/videos/fullstack-enterprise-mevn/9781800202276/9781800202276-video2_1)
