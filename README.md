## WVP-GB28181 2.0漏洞

这是一个关于WVP-GB28181 2.0 的逻辑漏洞
#### 可复现问题的步骤 The steps to reproduce.
The latest version of wvp GB28181 pro is 2.0. Let's first take a look at the effect of a normal page loading platform:
The password is weak password 123, and the account is shown in the picture

![图片3](https://github.com/guipi01/WVP-GB28181/assets/102499073/b520429f-ec5d-49eb-b595-fe5562bd9545)

Login successful. In the user management interface, when changing the password, change the value of userId to 1 and modify the password of the administrator account admin

![WechatIMG638](https://github.com/guipi01/WVP-GB28181/assets/102499073/218b512f-f375-4cf1-bd5f-f854f8f18783)

Modified successfully
![图片2](https://github.com/guipi01/WVP-GB28181/assets/102499073/5934c6e3-1f72-4771-ada9-97cd9c69138f)

Administrator admin account login successful


可复现问题的网页地址 Reproducible webpage address
[http://112.28.134.194:8088/#/login](url)
This website uses the latest version of wvp-GB28181 pro, and there are no users who can view any platform resources
受影响的Valine版本、操作系统，以及浏览器信息
Affected Valve versions, operating systems, and browser information

wvp-GB28181-pro 2.0
OS：Windows/Linux/macOS
Browser: Chrome、Firefox、Safair
总的来说，如果有普通用户成功越权到管理员权限，就会造成网站的敏感信息泄漏，希望作者大大后面可以修复这个问题。
Overall, if ordinary users successfully exceed their administrator privileges, it will cause sensitive information leakage on the website. We hope the author can fix this issue in the future.


参考链接：[https://github.com/648540858/wvp-GB28181-pro](url)
