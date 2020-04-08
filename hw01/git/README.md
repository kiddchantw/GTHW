https://github.com/SoJ0825/backendtraining-t1.git# 前言:
版本控制系統大概是最基礎的工具，不管你是在前端、後端還是 APP。熟悉 Git 是基本技能。假設你現在是一個人開發 Web 專案，你至少需要熟悉以下流程。

# 推薦學習資源
## 中文書：[為你自己學Git](https://gitbook.tw/)

# 問題
- Q1: 請說明
    1. 什麼是版本控制系統？

    	版本控制可記錄檔案內容變化，並且能夠查詢每個版本所更動內容。確保在軟體開發的過程，由不同人所編輯的同一程式檔案都得到同步。

    2. Git 版本控制中有哪幾種檔案狀態？

		不確定是指這四種狀態
		- untracked files ( 未追蹤 )  
		- changes not staged for commit （已更改） 
		- changes to be committed （等待提交） 
		- committed (已提交) 
	
		還是位在不同區域以下四種區域的git檔案狀態 
	
		- working directory  ( 工作資料夾） 
		- staging area (暫存區)  
		- local repo (本地端檔案庫)  
		- remote repo （遠端檔案庫） 
	
 
 


![](https://i.imgur.com/hZoDAPf.png)
- Q2: 上圖 A-J 是 Git 中檔案狀態切換得流程，請查出 A-J 執行的指令。(重點是確保自己真的學到在什麼情況下使用該指令。)
    - A: 將一般目錄變成 git working folder

		git init
	- B: 將 working folder 的異動狀態登錄到 stage 

        git add
	- C: 將 stage 的狀態放到 local repository 

	   git commit 
	- D: 將 local repository 的狀態放到 remote repository 

	 	git push
	- E: 將 remote repository 的狀態取回到 local repository 

		 git fetch
	- F: 將 local repository 的狀態退回到 stage 階段（是 C 的逆向）

		 git reset
	- G: 將 stage 的狀態退回到 working folder 階段（是 B 的逆向） 

		 git check out 
	- H: 將 local repository 的狀態一口氣退回到 working folder 階段（是 B+C 
	 的逆向） 
	 
	 	git revert
	- I: 從 remote repository 取回建立成新的 working folder 
	 
	 	git pull

 	- J: 將 git working folder 變回一般目錄
		
		git rm




- Q3. 做這個題目，你事前評估做了什麼、利用了哪些資源、排程為何、事後怎麼驗收、得到什麼經驗？


