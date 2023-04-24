# show-location-on-chatgpt

在 ChatGPT 首页显示当前所处 IP 和 Location，使用 OpenAI 官方接口查看代理节点被 OpenAI 识别成的国家，如果不再支持的国家，则会进行提示以免被封号。

下载地址：xxx

## 初衷

我们知道，现在 ChatGPT 的管控越来越严了，为了避免好不容易申请到的账号被 ban，我们最好是将我们的代理节点定位到 OpenAI 支持的国家，但是每次切换代理后，再去网站查看位置的过程太麻烦，如果在打开 ChatGPT 网站一眼能看到当前代理所在国家地区，以及是否是 OpenAI 支持的国家地区岂不美哉~

第二个原因是看到网上那么多从未接触过的人都开发了自己的浏览器插件或者 Tampermonkey 扩展，自己却从来没试过，那么正好有这个契机，让我从练练手。

## 个人知识背景

- 前端开发
- 对 Tampermonkey 扩展开发零基础

## 开发经过

- 基本上没有用到前端知识储备，只有提需求，然后将代码拷贝到 Tampermonkey
- 提问的过程全程使用英文（为了提高回复速度和正确率），对话过程如下（https://shareg.pt/fGk2bom），到最后的时候出现了小插曲，ChatGPT忘记了之前的对话，所以我重新把它的回答喂给他，然后基于此继续提需求。
- 原理很简单，就是根据 https://chat.openai.com/cdn-cgi/trace 接口返回所在国家，然后去匹配 OpanAI 官方宣布的支持的国家地区。
- show-location-on-chatgpt 扩展总开发时间：1 小时

## 成果截图

![image](https://user-images.githubusercontent.com/23518990/233934605-484c2613-df84-464d-a62d-bc66f710c6e2.png)

（Japan显示红色是我故意测试用的，实际会显示绿色）
![image](https://user-images.githubusercontent.com/23518990/233934890-113ad476-d3b1-4d3c-bc8f-0f90d95c7949.png)

