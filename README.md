# CUPS\_LanguagePackage\_zh\_CN
CUPS简体中文Web界面和在线帮助文档  
基于 CUPS 2.3.1, Ubuntu 20.04.3 TLS

# 简易安装方法
\# 复制汉化Web模板  
sudo cp -rp ./templates/zh\_CN /usr/share/cups/templates/  
sudo chown -R root:root /usr/share/cups/templates/zh\_CN/  
sudo chmod 755 /usr/share/cups/templates/zh\_CN/  
sudo chmod -R 644 /usr/share/cups/templates/zh\_CN/\*  

\# 复制汉化首页和帮助文档  
sudo cp -rp ./doc-root/zh\_CN /usr/share/cups/doc-root/  
sudo chown -R root:root /usr/share/cups/doc-root/zh\_CN/  
sudo chmod 755 /usr/share/cups/doc-root/zh\_CN/  
sudo chmod -R 644 /usr/share/cups/doc-root/zh\_CN/\*  
sudo chmod 755 /usr/share/cups/doc-root/zh\_CN/help /usr/share/cups/doc-root/zh\_CN/images  

\# 重命名原英文帮助文档目录  
sudo mv /usr/share/cups/doc-root/help /usr/share/cups/doc-root/help\_en  

\# 建立 help 的软链接实现中英文切换  
cd /usr/share/cups/doc-root  
sudo ln -s zh\_CN/help help  

# 关于汉化
汉化通过百度翻译/有道翻译机译完成，并辅以简单整理，难免有不准确或是不通顺之处，仅希望对您会有一点点的帮助。

