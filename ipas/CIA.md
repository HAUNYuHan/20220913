# CIA
- C 機密性(Confidentiality)
```
為了維持資訊在傳輸、儲存、處理狀態時，不被非授權人員存取、使用、竄改。
不該看的人看不到。
ex 客戶資料 薪資外洩
```
- I 完整性(Integrity)
  - 可歸責性 (Accountability) → 確保實體之行為可唯一追溯到該實體的特性。
  - 鑑別性 (Authenticity) → 確保一主體或資源之識別就是其所聲明者的特性。
                          → 適用於如使用者、程序、系統與資訊等實體。
```
只有具備權限的人可以修改資料內容，確保資料能維持原本的面貌，資料經時空變化，
內容也應該要能維持一致性，來確保資料的完整性。
內容未被竄改。
ex 合約 打卡紀錄被竄改
```
- A 可用性(Availability)
```
確保資訊系統能提供正常服務。
可用性必須與完整性極機密性之安全需求配合，並依照整體考量以符合資訊安全的目標
要可以正常使用。 (能用但很慢的話? 品質問題)
ex 訂票系統當機
```
# 3A

- 驗證(Authentication) 
- 授權(Authorization) 
- 可歸責(Accountability)

# 其他資安基本觀念

- 可靠度(Reliability)→ 始終如一預期之行為與結果的特性。
- 不可否認性(Non-repudiation)→ 對一已發生之行動或事件的證明，使該行動或事件往後不能被否認的能力。
- 邊界與分類(Boundary and classification)
- 職務區隔(Segregation of duties, SOD)
- 縱深防禦(Layered defense, defense in depth)
- 單一脆弱點(Single point of failure, SPOF)
- 阿奇里斯腱(Achilles heel)
- 木桶理論(Bucker principle）
- 僅知原則(Need to know)
# 108年 - 108-2 資訊安全工程師_初級
```
1. 關於搜尋引擎攻擊（Google-hacking），主要在破壞資訊系統的何種特性？
*(A) 機密性（Confidentiality）
(B) 完整性（Integrity）
(C) 可用性（Availability）
(D) 責任性（Accountability）
```
```
google-hacking是常見資料列舉的方法，透過google搜尋找到敏感資料或是與目標有關資訊。 
google只是查找，並不引響系統的完整性，也不會造成系統無法使用
```
```
2. 請問「對資料修改權的約束與限制，只有擁有權限的使用者才能修改」 所代表的意義是下列何者？
(A) 機密性（Confidentiality）
*(B) 完整性（Integrity）
(C) 可用性（Availability）
(D) 可讀性（Readability）
```
```
3. 關於將資料設定為「唯讀」之目的，下列敘述何者正確？
(A) 是為了確保資料之機密性
(B) 是為了確保資料之可用性
*(C) 是為了確保資料之完整性
(D) 是為了確保資料之可讀性
```
```
10. 在進行資產分級評估時，如果資訊系統服務中斷，將造成組織營運出現 重大影響，此狀況屬於下列何種評估面向？
(A) 機密性
(B) 完整性
*(C) 可用性
(D) 流動性
```
```
22. 勒索病毒（Ransomware）使用對稱式加密技術與非對稱式加密技術來 進行加密電腦內的檔案，
讓使用者無法使用，此現象主要影響資訊系統的何種特性？
(A) 機密性（Confidentiality）
*(B) 可用性（Availability）
(C) 完整性（Integrity）
(D) 鑑別性（Authenticity）
```
```
30. 憑證記載了個人資料、公開金鑰、憑證單位名稱、數位簽章、以及憑證 有效期限及用途等資訊，下列何者「不」是它的特性？
(A) 完整性（Integrity）
(B) 不可否認性（Non-Repudiation）
(C) 身分識別（Authentication）
*(D) 可用性（Availability）
```
```
可用性availability的部分是指：確保資訊系統能提供正常服務。
```
```
32. 遠端用戶撥入驗證服務（Remote Authentication Dial In User Service , RADIUS）是 AAA 三種服務的網絡傳輸協議
，關於此 AAA，下列何 者「不」正確？
(A) Authentication
(B) Authorization
*(C) Access
(D) Accounting
```
# 109年 - 資訊安全管理概論
```
1. 下列何者為「公司網路系統必須 24 小時運作」的主要原因？
(A) 機密性
*(B) 可用性
(C) 完整性
(D) 不可否認性
```
```
33. 關於可歸責性（Accountability）的定義，下列何者正確？
(A) 對使用者所提出的可識別資訊加以驗證
(B) 使用者必須提供可識別的資訊給系統
*(C) 成功登入系統後，對於使用者的操作行為必須完整的記錄
(D) 管理階層的管理機制，將管理工作分成多人分層負責
```
# 110年 - 110-1初級資訊安全工程師
```
1. 關於資訊安全「可用性」的定義，下列敘述何者正確？
(A) 確保資訊的正確和完全性
*(B) 確保資訊在需要時可被存取和使用
(C) 確保資訊在傳輸過程中已確認兩方的身分和合法性
(D) 確保資訊不會被揭露或被未經授權的個人、實體和流程所取得
```
```
35. 下列何者「不」是應用系統安全防護的三大核心（AAA）？
(A) Authentication
(B) Authorization
*(C) Availability
(D) Accounting
```
# 110年 - 初級資訊安全工程師能力鑑定：資訊安全技術概論
https://app.yamol.tw/exam/102069
