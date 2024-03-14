# Mac_switch_JDK


# Mac_switch_JDK

### 查看电脑上所有Java的版本

`/usr/libexec/java_home -V`

![image-20240314161315944](/Users/suer/Library/Application Support/typora-user-images/image-20240314161315944.png)

### 查看当前Java版本

java -version

![image-20240314161423912](/Users/suer/Library/Application Support/typora-user-images/image-20240314161423912.png)

### 切换版本

```
*# 切换到 1.8*
 export JAVA_HOME=`/usr/libexec/java_home -v 1.8`
 *# 切换到 17* 
export JAVA_HOME=`/usr/libexec/java_home -v 17`
```

### 设置成全局

```
vim ~/.bash_profile
## 最后一行新增
export JAVA_HOME=`/usr/libexec/java_home -v 1.8`
## 然后更新配置
source ~/.bash_profile
## 解决在 zsh 终端中失效的问题
## zsh中
vim ~/.zshrc
## 在~/.zshrc文件最后，增加一行：
source ~/.bash_profile        
## 执行命令，使其立即生效
source ~/.zshrc  
```

