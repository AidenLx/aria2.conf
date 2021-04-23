# 安装

<https://p3terx.com/archives/aria2-frontend-ariang-tutorial.html>

添加aria2.session

```sh
touch ~/.aria2/aria2.session
```

## brew自启动

```sh
echo '<!--?xml version="1.0" encoding="UTF-8"?-->
<plist version="1.0">
    <dict>
<key>Label</key>
<string>homebrew.mxcl.aria2</string>
<key>ProgramArguments</key>
<array>
<string>/usr/local/opt/aria2/bin/aria2c</string>
</array>
<key>RunAtLoad</key>
<true/>
<key>KeepAlive</key>
<true/>
</dict>
</plist>' > /usr/local/opt/aria2/homebrew.mxcl.aria2.plist
```
