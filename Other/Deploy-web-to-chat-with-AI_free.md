# 准备
## 账号
1. GitHub账号，[官网](https://github.com/)
2. Cloudflare账号，[官网](https://cloudflare.com)
3. Vercel账号，[官网](https://vercel.com)
4. 免费域名(*.us.kg)，[注册](https://register.us.kg/)，网络上有教程。通过身份验证的话可以使用[身份生成器](https://www.meiguodizhi.com/)
## 软件
1. Git ~~虽该教程无用，但是很好的工具，望能了解并使用，跨平台，与GitHub等网站相结合使用。 ~~[官网(含教程)](https://git-scm.com/)

# 以[NeatChat](https://github.com/tianzhentech/NeatChat)为例
## Fork
去GitHub中将该项目fork到个人的GitHub仓库中，~~自行Google~~
## 打开[Vercel](https://vercel.com)网站
登录后点击`Add New`按钮，在展开菜单中选择`Project`。

然后连接到GitHub，将刚刚fork的项目import进去，默认即可，点击`Deploy`。等待部署结束
**注**：若要自定义模型(添加没有的)请去环境变量中添加`CUSTOM_MODELS`项，具体请看[文档](https://github.com/ChatGPTNextWeb/NextChat?tab=readme-ov-file#custom_models-optional)

## 打开[us.kg](https://register.us.kg/)网站
登录，并访问[该网址](https://dash.domain.digitalplat.org/panel/main)注册一个免费域名(注：需要续期，但续期免费，在“我的域名”详情页即可看见。)

### 打开[Cloudflare](https://cloudflare.com)网站
登录后点击`Add a domain`，将要申请的`us.kg`网址填写进去(要写全，如`pilihu.us.kg`)。然后选择免费计划，将选项中的`始终使用HTTPS`打开，一直下一步直到提示填写`Name Server`。

将Cloudflare中显示的两个`Name Server`填写到`us.kg`网站申请处即可。

## 前往Vercel
检查是否成功部署好[NeatChat]，成功后前往`Settings`处，点击`Domains`，点击`Add`按钮，**完整地**输入你想要添加的域名(如`chat.pilihu.us.kg`，建议添加子域名。)

然后根据提示，前往Cloudflare网站，点击进你申请的域名，点击左侧菜单的`DNS`按钮，然后点击`Add record`，按照Vercel的提示添加即可。

# 调用API
## 以硅基流动为例
电脑前往[官网](https://siliconflow.cn/zh-cn/)。登录后访问[申请API key](https://cloud.siliconflow.cn/account/ak)。创建后复制好。

## 使用
访问绑定好NeatChat的域名，点击页面左下角的齿轮图标，进入设置页面。

然后找到`自定义接口`开关，打开，将`服务提供商`选择为`OpenAI`。

将**接口地址**替换，并填写为
```
https://api.siliconflow.cn/
```

然后填写好下方的`API Key`。

在`自定义模型`一栏中填写好你想用的模型(如DeepSeek)
```
deepseek-ai/DeepSeek-V3,deepseek-ai/DeepSeek-R1
```
**注**：若使用R1模型来询问问题，发现一直在加载动画，请不要怀疑，它正在思考。
然后只需要点击新的聊天，并直接开始。切换模型则点击![image.png](https://s2.loli.net/2025/02/12/4WcpmtSdDoHX7hn.png)
若想看见思考内容，请~~等我研究研究~~
