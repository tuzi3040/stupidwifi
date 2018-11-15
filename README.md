> # 某皇家气象学院校园wifi一键登录
---
> ## Info
* python2.7
    * requests
    * json
    * base64
    * time
    * os
* VScode
  

> ## Version
* 更新:2018.11.16
* Version: 1.0

* 更新内容:
    * 区分了linux版本,和win版本
    * win版本下加上了检查wifi链接情况
    * 修复了linux下脚本路径的问题
    * 修改了一下下界面
*  **linux下没有自动连接wifi功能,仅实现了web认证(原因是没有找的合适的库又懒得造轮子)**

> ## Usage
* Windows
    * 已打包生成了exe文件
    * 直接双击运行,第一次会要输入web认证信息,之后信息会被保存
    * 以后使用只需要双击exe即可
    * PS无需保证wifi是否已经连接上,程序自身会检查wifi连接
    * 但是请确保您不是第一次连接i-NUIST

* linux
    * 在sample.py目录下运行该脚本
         ```
         python sample.py
        ```
        sample.py可以是你修改的该脚本的名字
    * 使用alias命令
        
        * 编辑root目录下的.bashrc文件,添加(sample.py是该脚本名字)
        ```
        alias   inuist="python /root/sample.py"
        ```
        
        * 保存退出后运行
        ```
        source .bashrc
        ```

        * 接下来只要在命令行运行,即可连接wifi一键认证
        ```
        inuist
        ```

 ### **linux下没有自动连接wifi功能,仅实现了web认证(原因是没有找的合适的库又懒得造轮子)**