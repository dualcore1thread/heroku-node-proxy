## 基于node unblocker的通用web代理
本工程是 [node-unblocker](https://github.com/nfriedly/node-unblocker) 的一个副本，只是修改了工程结构，以便于直接在Heroku上部署;  原作者的版本里, 所有的代理请求被到 http, 在这种场景下, URL中含有敏感域名会导致连接被GFW重置。因此，在该副本里，修改了代码让所有代理请求全使用https。

# 一键部署，请点击下方的"Deploy to Heroku"按钮

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

# 常见问题

网站不能被打开，显示链接被重置：本品没有设置自动https访问，GF。W升级过后，会检测访问链接来屏蔽某些敏感链接，某些设备可能会出现这种情况，遇到此问题时，请使用强制https访问的方法，就可以解决。同时，没有此问题的用户也强烈建议您使用强制https访问，安全性更高，不易被封。

# 注：此代理适用于大多数网站，但无法播放YouTube视频。观看YouTube视频，请使用 [you2php-heroku](https://github.com/zhangke200377/you2php-heroku)。
