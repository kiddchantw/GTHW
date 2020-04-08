# 前言
相信大家看過很多電影裡面的帥氣駭客們，總是在黑底白字的介面前面輸入指令操控著電腦。 身為一個工程師，我們當然也要立志當帥氣的工程師，既然如此就得好好學學怎麼使用這烏漆抹黑的介面。

# 推薦學習資源
[鳥哥的 Linux 私房菜](https://linux.vbird.org/linux_basic/centos7/)

# 問題

### 名詞解釋

- GUI vs CLI

    GUI :  圖形化使用者介面(Graphical User Interface)  e.g. window10
    CLI :   文字指令行介面(Command Line Interface)  e.g. termimal

- terminal

    macOS中的終端機、CLI 的一種輸入輸出界面

- shell 

    殼程式 (shell)  =  應用程式 ，是提供使用者操作系統的介面
 
    - bash

         Linux 預設的 shell

    - zsh 

        預設使用bash shell 的linux shell，可擴充性較高
    
### 請解釋下方 CLI 的指令作用
    
- `cat`

    - 將檔案內容文字化，顯示/印出在螢幕上

    - 合併多個檔案到最後一個指定的檔案中
- `cd`

    改變當前工作目錄位置
    
- `chgrp`

    改變檔案所屬群組

- `chown`

    改變檔案擁有者

- `chmod`
    
    改變檔案的權限

- `cp`
    
    複製檔案

- `curl`

    利用URL規則在命令列下工作的檔案傳輸工具
    
    支援檔案的上傳和下載

    基本用法  用於測試一臺伺服器是否可以到達一個網站 （安裝linux的時候很多時候是沒有安裝桌面的)

    儲存訪問的網頁

    測試網頁返回值

    指定proxy伺服器以及其埠port

    處理cookie  : 增加相關引數可快速處理

    模仿瀏覽器

    偽造referer(盜鏈)

    斷點續傳

    顯示抓取錯誤

- `grep`
    
    grep 則是分析一行訊息， 若當中有我們所需要的資訊，就將該行拿出來

    使用關鍵字或正規表示法（regular expression）篩選出想要尋找的資料，並且顯示出來

- `less`
    
    查看文件

- `ls`
    
    查看目錄

- `man`
    UNIX/Linux 系統中的指令都會附帶相關的線上說明手冊(manual操作說明)，提供使用者查詢與參考。

- `mkdir`
    建立目錄folder   

- `mv`

    改變檔案的名稱

    搬移出目前位置

- `|`

    管線 (pipe)：分隔兩個管線命令的界定。    
    『 | 』僅能處理經由前面一個指令傳來的正確資訊，也就是 standard output 的資訊，對於 stdandard error 並沒有直接處理的能力。


- `pwd`

    印出目前工作目錄的名稱
- `rm`

    刪除檔案或目錄
- `touch`

    建立檔案file
- `vim`

    編輯file


### 請說明以下 Linux file system structure 

- `/`

用 / 切隔目錄名  
root 根目錄
- `/bin`

需要在單用戶模式可用的必要命令（可執行檔）；面向所有用戶，例如： cat、 ls、 cp。
- `/etc`

特定主機，系統範圍內的設定檔。
- `/home`

用戶的家目錄，包含儲存的檔案、個人設定等，一般為單獨的分割區。
- `/lib`

/bin/ 和 /sbin/中二進位檔案必要的庫檔案。
- `/var`

變數檔案——在正常執行的系統中其內容不斷變化的檔案，如紀錄檔，離線檔案和臨時電子郵件檔案。有時是一個單獨的分割區。
- `/sbin`

必要的系統二進位檔案，例如： init、 ip、 mount。
- `/srv`

/srv ：主要用来存储本机或本服务器提供的服务或数据。（用户主动生产的数据、对外提供服务）
- `/tmp`

臨時檔案(參見 /var/tmp)，在系統重新啟動時目錄中檔案不會被保留。
- `/usr`

用於儲存唯讀用戶資料的第二層次； 包含絕大多數的(多)用戶工具和應用程式，注意不是user的縮寫，而是"Unix Software Resource"的縮寫。