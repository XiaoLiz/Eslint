# Configuring ESLint 

ESLint
可组装的JavaScript和JSX检查工具

也可理解为：ESLint是一个用来识别 ECMAScript 并且按照规则给出反馈的代码检测工具，可以避免错误和统一代码的风格。


<br>
### 安装（install）

全局安装: 

``` $ npm install -g eslint ```
<br>

项目局部安装: 

``` $ npm install eslint --save-dev ```  或者简写  ```$ npm i -D eslint ```

如果安装报错，加上sudo 权限安装即可如：

``` $ sudo npm install -g eslint ```

<br>
生成eslint.js配置文件：

``` $ eslint --init ```
<br>
  ```
  {
      "rules": {
        "quotes": [
            "error",
            "single"
        ],
        "semi": [
            "error",
            "always"
        ]
    }
  }
  ```  

  
<br>

`注意`：eslint --init适用于对某个项目进行设置和配置 ESLint，并在其运行的的目录执行本地安装的 ESLint 及 插件。如果你倾向于使用全局安装的 ESLint，你配置中使用的任何插件也必须是全局安装的。


### 配置（config rules）

配置的信息主要分三种情况：

```
  Environments - 指定脚本的运行环境。每种环境都有一组特定的预定义全局变量。

  Globals - 脚本在执行期间访问的额外的全局变量

  Rules - 启用的规则及各自的错误级别
```


  
  <br>
在配置文件中可以设置一些规则。规则的等级有三种：

  "off" 或者 0：关闭规则。
  
  "warn" 或者 1：打开规则，并且作为一个警告
  
  "error" 或者 2：打开规则，并且作为一个错误




  <br>
  <br>
  
### 参考资料
- [eslint](https://githuab.com/eslint/eslint)
- [eslint-config](https://github.com/AlloyTeam/eslint-config-alloy)


