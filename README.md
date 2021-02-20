## 一份优雅简约的在线简历
- 优化构建，页面秒开无闪烁
- 自适应屏幕兼容移动端
- 支持部署到ghpages，可在线浏览
- 自动生成 PDF，全自动化流程

## 使用
1. 项目依赖于 Node 环境，你需要先到 Node 官网[2] 下载并安装对应系统的 Node 程序。安装好后，在命令行输入 node -v，如果出现相应的版本号，说明 Node 环境安装成功。

2. fork本项目到你的GitHub仓库中 后再使用Git工具Clone到本地修改。

3. 使用 CD 命令进入到项目目录，输入`npm install`命令，安装程序所使用的依赖环境。

4. 再输入 `npm run dev` 命令，项目会进行编译，并自动打开浏览器，加载出简历的页面。

5. 打开编辑器对简历内容进行修改。

5. 项目的整体目录结构如下：
            
            `├── README.md
                ├── node_modules
                ├── package-lock.json
                ├── package.json
                ├── postcss.config.js
                ├── src
                ├── webpack-dist.config.js
                ├── webpack.config.js
                └── webpack.js`
            
7. 修改简历内容，直接编辑 `index.html` 文件。

8. 如果要修改简历的样式，比如主题色、字体等等，需要编辑 `main.css` 文件。

9. 简历修改完后，刷新一下浏览器就可以看到最新的内容。

11. 替换webpack-dist.config.js文件里的hshuai.xyz为你自己的域名，并根据该文档配置你的域名解析
（这一步如果你没有自己的网页，则把这一行注释，这样系统生成的GitHubpages则默认设置为网址https://yourname.github.io/MyResume/ 这个域名也可以用但是太low了，建议个人主页去买一个域名，阿里云新人域名一年一块钱很方便）

12. 回到项目，在命令行中先输入`cnpm install cross-env`再输入 `npm run pub` 命令，会自动创建一个 gh-pages 分支并推送到你fork的 GitHub 的仓库。

13. 打开上面 Fork 的仓库地址，点击设置，滑动到 `GitHub Pages` 设置选项，将分支选择为 `gh-pages`此时Github Actio已经自动给你部署好网站你需要去你个人域名页面解析该域名，具体方法请百度。

14. 然后打开生成的网页即可看到在线的简历，将链接发给其他人，其他人通过浏览器打开可以直接访问

15. 使用快捷键 `ctrl+p` 或者 `command+p` 调用浏览器的打印功能，可以将简历导出为 pdf 格式的文件。

