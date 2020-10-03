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
## 7.Installing the Tailwind CSS:
1.change in the latest version of Tailwind:
a. you need to cchange the plugins in the post.config.js to the code btaild.config.js:  
```
module.exports = {

    plugins: [require('tailwindcss')('./tailwind.config.js')]
}
```
2.add the default code to the tailwind.config.js
[tailwindlabs/tailwindcss](https://github.com/tailwindlabs/tailwindcss/blob/master/stubs/defaultConfig.stub.js)  
[Rename tailwind.js to tailwind.config.js](https://tailwindcss.com/docs/upgrading-to-v1#3-rename-tailwind-js-to-tailwind-config-js)  

3.[Error: Specified Tailwind config file "...\tailwind.js" doesn't exist. #19](https://github.com/JeffreyWay/laravel-mix-tailwind/issues/19)   
solution:  
```
it will generate a file tailwind.config.js. rename it to tailwind.js and run npm run dev again.
```

## 8. file search in visualstudio:
[How do I search for files in Visual Studio Code?](https://stackoverflow.com/questions/30095376/how-do-i-search-for-files-in-visual-studio-code)  

## 9. the reason why your text could not be link to a file:

You need to go to the .balerc file and locate the "plugins" code to add the @ to the pages: @pages.

## 10.When you meet webpack is not defined error:
You need to check the lowercase or uppercase of w in the webpack.


## 11.Design home screen:

1.[Upgrading from v0.x to v1.0](https://tailwindcss.com/docs/upgrading-to-v1#3-rename-tailwind-js-to-tailwind-config-js)    
2.[Google Fonts](https://fonts.google.com/specimenTab?standard-styles)  

## 12. Design register screen:
1. You need to click the join now button to see the color UI change.  

## 11.Custom input compoent:
[VueJs dev tools panel not showing](https://stackoverflow.com/questions/41505150/vuejs-dev-tools-panel-not-showing#:~:text=Try%20the%20following%3A,look%20for%20the%20Vue%20tab)

## Resource List:  
1.Project Resource List:[Fullstack Enterprise MEVN: Mongo, Express, Vue, and Node](https://learning.oreilly.com/videos/fullstack-enterprise-mevn/9781800202276/9781800202276-video2_1)  
2. Visul studio file icon extensition:[vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)  
3. Reference Code here:[PacktPublishing-Fullstack-Enterprise-MEVN---Mongo--Express--Vue--Node](https://github.com/sanjanapackt/PacktPublishing-Fullstack-Enterprise-MEVN---Mongo--Express--Vue--Node/blob/master/tailwind.js)  

