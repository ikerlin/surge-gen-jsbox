## surge-gen-jsbox

Surge3+配置管理器

### 安装

[点击安装](https://xteko.com/redir?name=Surge%20Policy&url=https%3A%2F%2Fgithub.com%2FFndroid%2Fsurge-gen-jsbox%2Fblob%2Fmaster%2F.output%2FSurge%2520Policy.box%3Fraw%3Dtrue)

### 特性
1. 支持多服务商订阅
2. 便捷的策略编辑操作
3. 第三方规则可视化更新

### 使用

1. 点击界面最上方“铅笔”按钮，导入基础配置文件，删除配置文件中不需要的节点（[Proxy]下）
2. 退回主界面，此时主界面会根据策略组进行刷新
3. 点击主界面最上方“云朵”按钮，添加服务商提供的托管地址，用于获取节点信息
4. 退回主界面，点击最上方“刷新”按钮，拉取节点信息
5. 根据自己的需求安排策略组，点击PROXIES下节点进行移除，点击MORE下节点进行添加
6. 点击Generate按钮尝试生成，如果无法生成，脚本会自动导航到节点不存在的策略组中，修复所有问题即可生成


### 更新配置

由于Surge3+支持RULE-SET可以远程下载规则，所以多数时间我们并不需要使用脚本修改规则

但是脚本中提供了一个DIFF工具，使用这个工具，可以将当前的配置文件和规则维护者的配置文件进行比较，并且选择需要的更新进行合并

#### 具体操作

1. 点击界面最上方“铅笔”按钮，打开基础文件编辑界面
2. 点击界面底部左边的按钮，输入远端配置文件地址，点击确定
3. 在打开的界面中，根据提示进行修改

提示类型：
- 绿色：本地文件增加内容
- 红色：远端文件多余内容

当点击提示时，对应的内容会被删除，当所有内容检查完毕后，点击Save按钮即可保存配置文件

> 此处操做类似于git diff
