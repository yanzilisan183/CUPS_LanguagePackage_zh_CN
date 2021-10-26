# CUPS_LanguagePackage_zh_CN
CUPS简体中文Web界面和在线帮助文档  
基于 CUPS 2.3.1, Ubuntu 20.04.3 TLS

# 简易安装方法
\# 复制汉化Web模板  
sudo cp -rp ./templates/zh_CN /usr/share/cups/templates/

\# 复制汉化首页和帮助文档  
sudo cp -rp ./doc-root/zh_CN /usr/share/cups/doc-root/

\# 重命名原英文帮助文档目录  
sudo mv /usr/share/cups/doc-root/help /usr/share/cups/doc-root/help_en

\# 建立 help 的软链接实现中英文切换  
cd /usr/share/cups/doc-root  
sudo ln -s zh_CN/help help

# 关于汉化
汉化通过百度翻译/有道翻译机译完成，并辅以简单整理，难免有不准确或是不通顺之处，仅希望对您会有一点点的帮助。

