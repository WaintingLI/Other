Mkcert安裝  
===
>需事先安裝"chocolatey"
> 他是在Windows環境下,Pack Manager,就像Ubuntu底下的apt一樣  
> 主要參考:[使用mkcert輔助，以HTTPS模式開發網頁](https://reginnachao.medium.com/%E4%BD%BF%E7%94%A8mkcert%E8%BC%94%E5%8A%A9-%E4%BB%A5https%E6%A8%A1%E5%BC%8F%E9%96%8B%E7%99%BC%E7%B6%B2%E9%A0%81-d978d1bc8e01)
---

1. cmd,輸入 **"choco install mkcert"**


2. 安裝本機憑證,輸入 **"mkcert -install"**  
*※備註:移除本機憑證,請輸入"mkcert -uninstall"*

3. 安裝完成後,會在以下各路徑找到該憑證:  
> - macOS：檔案會安裝於 /Users/***/Library/Application Support/mkcert  
> - Windows：檔案會安裝於C:\Users\User\AppData\Local\mkcert


4. Windows下,將"rootCA.pem"改為"rootCA.crt",就可以安裝該憑證

5. 藉由輸入" mkcert "\*.k8s.local" "來創建,.pem與key.pem來安裝憑證


  
  
參考網址:  
- [使用 mkcert 製作本機憑證](https://mileschou.me/blog/mkcert/)
- [SSL 憑證製作與匯入](https://ithelp.ithome.com.tw/articles/10282250)
- [使用mkcert輔助，以HTTPS模式開發網頁](https://reginnachao.medium.com/%E4%BD%BF%E7%94%A8mkcert%E8%BC%94%E5%8A%A9-%E4%BB%A5https%E6%A8%A1%E5%BC%8F%E9%96%8B%E7%99%BC%E7%B6%B2%E9%A0%81-d978d1bc8e01)
- [使用mkcert生成SSL证书](https://blog.csdn.net/qq_45994827/article/details/129850627)