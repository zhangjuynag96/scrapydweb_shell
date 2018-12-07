# 文档是scrapyd与scrapydweb的部署说明

# 脚本文件是用来自动安装scrapyd与scrapydweb的
## 运行脚本文件后scrapyd与scrapydweb都会自动运行.可以使用

> ps -ef | grep scrapyd
> ps -ef | grep scrapydweb

## 找到进程PID，然后杀死进程.有关scrapydweb的配置可以在脚本文件中的install scrapydweb模块中修改.修改方法在文档中有.
### 不要在scrapydweb_settings_v4.py文件中修改，脚本会自动覆盖，当然你也可以在脚本中禁用自动运行scrapydweb（注释掉scrapydweb_run模块下的代码即可.)
### 注释掉scrapydweb_run模块后，即自行修改scrapydweb_settings_v4.py配置文件,自行启动scrapydweb即可.

### 运行配置文件都在当前目录下新建的WorkSpace 文件夹中
