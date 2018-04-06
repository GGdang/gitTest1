# gitTest
## git指令練習

git version                                     版本查詢  
git config --list                               查詢設定列表  
git config --global user.name '名字'            設定名字  
git config --global user.email 'email'          設定e-mail  

git init                                        把資料夾變成git資料夾  

git add .                                       提交全部檔案到索引中  
git add abc.txt                                 提交單一檔案  

git reset head                                  取消全部索引檔案  
git reset head abc.txt                          取消單一索引檔案  

git status                                      查詢提交狀態  

git commit -m '訊息'                            把索引檔案送出並做下紀錄  
git log                                         查詢提交紀錄訊息  

git checkout 檔案名字                            檔案還原到最新的更新狀態(單一檔案)  
git reset --hard                                 還原工作目錄與提交狀態，會更最後一次commit保持一樣

git clone 網址                                   把遠端資料庫跟本地作連結  
git push                                         若有連結遠端數據庫的話，可以更新遠端資料庫的資料  

HEAD:指標  
git branch                                       查詢分支  
git checkout 前4個編碼(commit編碼)                將分支移動到選擇的commit紀錄上  
git checkout 分支名稱                             移動HEAD到指定的分支上  
git branch 分支名稱                               新增分支  
git merge 分支名稱                                合併分支的更新 ps:需切換到要合併的分支上 ex:master 要合併 featrue1的話，需移動到master上   

tag:標籤  
git tag                                          查詢標籤  
git tag -n                                       查詢標籤詳細內容  
git tag 標籤名稱                                  新增標籤 單純加標籤  
git tag -am '備註內容' 標籤名稱                    新增標示標籤 加標籤也加內容  
git tag -d 標籤名稱                               刪除標籤  
tag checkout 標籤名稱                             切換到標籤的commit  

暫存目錄  
git stash                                         暫時儲存當前目錄  
git stash list                                    瀏覽 git stash 列表  
git stash pop                                     還原暫存  
git stash drop                                    清除最新暫存  
git stash clear                                   清除全部暫存  

推送分支到遠端資料庫  
git remote                                        查詢遠端數據庫
git remote rename 原名稱 修改名稱                  修改數據庫名稱 
git push 遠端主機名稱 分支名稱                      若有連結遠端數據庫的話，可以更新遠端資料庫的資料，但有時會有很多遠端數據庫，所以請指定要送至哪一個數據庫  

git pull                                          更新遠端數據庫的資料到本機中  
git fetch 遠端主機名稱 分支名稱                     
