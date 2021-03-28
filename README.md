# Cloud189Checkin
天翼云盘每日签到一次，抽奖2次  
##### 直接调用
1.下载或通过git克隆项目 
2.测试环境为python3.7.6,自行安装python3  
3.requirements.txt 是所需第三方模块，执行 `pip install -r requirements.txt` 安装模块  
4.可在脚本内直接填写账号密码  
5.Python 和需要模块都装好了在项目所在目录 cmd 中执行``python C189Checkin.py ``

登录看的以下项目：
> [Cloud189](https://github.com/Dawnnnnnn/Cloud189)
> [cloud189](https://github.com/Aruelius/cloud189)

# Github Actions说明
## 一、Fork此仓库
![](http://tu.yaohuo.me/imgs/2020/06/f059fe73afb4ef5f.png)
## 二、设置账号密码
添加名为**USER**、**PWD**、**SCKEY**(可选)的变量  
值分别为**账号**、**密码**、**Server酱的KEY**  
多账号时账号密码一行一个一一对应  
示例：  
**USER**
```
123456
24678
```
**PWD**
```
cxkjntm
jntmcxk
```
**SCKEY**  
KEY获取方法详见官网：https://sc.ftqq.com

```
xxxxxxxx
```
![](http://tu.yaohuo.me/imgs/2020/06/748bf9c0ca6143cd.png)
![](http://tu.yaohuo.me/imgs/2020/06/af2013b1ef5d8430.png)
![](http://tu.yaohuo.me/imgs/2020/06/09c22adcec7b5d81.png)


## 三、启用Action
1.点击**Action**，再点击**I understand my workflows, go ahead and enable them**  
![Enable Actions](http://tu.yaohuo.me/imgs/2020/06/34ca160c972b9927.png)
2.点击**Enable workflow**
![Enable workflow](https://tu.yaohuo.me/imgs/2020/12/bfbae0a0f094daf1.jpg)
3.在[ Actions > Cloud189Checkin > Run workflow ]手动运行一次  
![Run workflow](https://tu.yaohuo.me/imgs/2020/12/3ac171041a7f730e.png)

## 四、查看运行结果
Actions > Cloud189Checkin > build  
能看到如下图所示，表示成功  
![](https://tu.yaohuo.me/imgs/2020/12/fd318c951e1c9b3b.jpg)

此后，将会在每天10:00-10:45之间和22:00-22:45之间各签到一次  
若有需求，可以在``.github/workflows/run.yml``中的``cron``自行修改

## 可能遇到的问题
* 验证码错误  
* 首先考虑是不是密码错误  
* 其次查看是否已经关闭设备锁  
