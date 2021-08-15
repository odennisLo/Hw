# 請說明什麼是git Sub-module,使用時機與實際演練該如何使用?
* 說明:Submodule 是用像指標的方式，將 SubRepo 的 HASH 紀錄在 SuperRepo 中。
* 使用時機:在專案底下，需要將其他人的專案掛載在自己任何目錄底下。
* 如何使用: 
  1. git submodule add (repo url) (folder)
  3. git commit
  4. git push