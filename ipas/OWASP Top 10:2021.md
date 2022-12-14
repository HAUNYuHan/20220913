![image](https://user-images.githubusercontent.com/71476327/195991521-23e9dc34-b303-4ca1-84df-dea05bb8f2e2.png)
# 什麼是OWASP？
- 是由「開放式Web應用程式安全專案 (OWASP) 基金會」，針對 Web應用程式漏洞和攻擊趨勢進行深入研究，建立了一套軟體安全行業指南和標準。
- 其中，OWASP Top 10 是最受歡迎和使用最廣泛的Web應用程式安全意識指南。
- 而這份列表也成了當前十個最關鍵的Web安全風險指標。

## 1 Broken Access Control 權限控制失效
- 權限控制失效是指訪問控制策略未能將帳號限制設定為預期的權限，容易讓駭客透過這項漏洞，
  進入企業中查看、修改、洩露、刪除其他帳號和管理員的數據，或是修改帳號和權限，甚至將惡意軟體安裝到系統中。
- 比之前的排名上升了四位，Broken Access Control（權限控制失效）成為最關鍵的 Web應用程式安全風險，超過 94% 的應用程式易受攻擊。

- 預防：為了保護應用程式免受駭客攻擊訪問，企業應預設拒絕訪問功能並設定身份驗證。

## 2 Cryptographic Failures 加密機制失效
- 加密機制失效在 2017 年列表中稱為敏感資料外洩。名稱在2021年重新定義，並將問題核心定義在加密機制的失敗，
  並且因此而造成敏感性資料外洩或是系統被破壞。
- 此外，它還表示為密碼保護不再足夠，並且預設情況下應該對所有包含敏感信息的數據庫應用加密。

- 預防：因手動加密在現在複雜的解密工具面前往往很弱，所以防止加密機制失效的最佳方法是使用受信任的加密解決方案。

## 3 Injection 注入式攻擊
- 注入式攻擊是最古老的、部署最廣泛的 Web 攻擊之一，94% 的應用程式易受攻擊，之前獨立排名的跨站腳本(XSS)也被合併到了注入式攻擊中。
- 在注入式攻擊中，駭客將惡意代碼注入系統以啟動未經授權的命令來取得敏感數據。
- 注入式攻擊的列表很長，包括 SQL 注入、跨站點腳本 (XSS)、模板注入、XPath 注入、電子郵件標頭注入、shell 注入等。

- 預防：為防止注入式攻擊，軟體開發人員應取消用戶提供的密碼輸入，
  並用行動 OTP（政府系統，銀行皆已廣泛使用）、生物識別身份驗證、下拉式選項和使用第三方支付平台來取代。
- 事實上，這聽起來可能很簡單，但對企業來說都很難實施。
- 因此，另一種更方便的方法是使用 Web 應用程式防火牆 (WAF)。Penta Security 的 WAF 產品 WAPPLES 是使用 AI邏輯檢測引擎來分析 HTTP 和 HTTPS 流量內容，保護您的 Web應用程式、API 和行動 APP，避免遭受惡意攻擊。

## 4 Insecure Design 不安全設計
- 不安全設計是 2021 年列表中新增的一項，定義了與應用程式設計缺陷相關的風險。
- 這些不一定是設計錯誤，而只是有心人士可利用了能造成損害的漏洞。
- 而這和不安全的配置卻相混淆。舉個簡單的例子；網站允許前 1,000 名獨立訪問者獲得折扣。
- 有心人士卻使用不同的 IP 位置購買多種打折產品並轉售以獲取收益。

- 預防：建議軟體開發人員使用安全的設計模組和參考架構來構建應用程式。
- 企業應該存儲這些安全模組和參考數據庫以備將來使用，在最終確定設計之前對應用程式執行威脅模式和滲透測試。

## 5 Security Misconfiguration 安全設定缺陷
- 0% 被測試的應用程式都有驗測到某種類別的安全設定缺陷，在前一個版本中的 XML 外部實體注入攻擊 (XML External Entities)被合併於這個類別。
- 安全設定缺陷最常見原因是系統管理員沒有更改預設配置，或者他們在打開系統進行測試後忘記重新關閉系統。
- 例如，敏感數據暴露的主要原因之一是雲端存儲權限配置錯誤。

- 預防：為了防止安全設定缺陷，企業應禁用所有預設的不必要功能、特權和權限，並僅開放給特定對象使用。每次安裝更新或補丁時定期檢查系統配置也很重要，重點是雲端服務和存儲。

## 6 Vulnerable and Outdated Components 危險或過舊的元件
- 在之前標題為使用有已有漏洞的元件。
- 危險或過舊的元件是指網路中的元件包含了未修補已知漏洞的情況，通常是過時且不受支援的操作系統、應用程式、Web 應用程式伺服器、API 和數據庫管理系統 (DBMS) 。

- 預防：消除危險或過舊元件的最佳方法是定期掃描漏洞並保持更新和修補所有軟體元件。
- IT 管理員還應管理軟體元件並刪除不必要的程式和功能。

## 7 Identification and Authentication Failures 認證及驗證機制失效
- 之前為排名第二的無效身份認證，將到第七位是因為越來越多企業組織採用多因素身份驗證 (MFA) 以及行動 OTP 和生物識別等高級身份驗證技術，這些技術都有助防禦社交攻擊、憑證填充和蠻力攻擊。

- 預防：在無法補救前，建議企業組織採用多因素身份驗證MFA，謝絕非法使用者進入大門。

## 8 Software and Data Integrity Failures 軟體及資料完整性失效
- 這是 2021 年版本全新的類別，軟體及資料完整性失效是由於缺乏資料完整性驗證過程而使用篡改或損壞的資料做出某些決定的狀況。
- 例如，駭客使用惡意軟體去破壞軟體更新文件，而應用程式會自動安裝更新，而無需驗證文件是否為原始文件。
- 這是影響全球數萬組織SolarWinds供應鏈攻擊事件的主要原因。

- 預防：為了防止資料損壞，建議使用 PKI憑證的驗證機制來確定資料的真實性和完整性。
- 對任何代碼或配置變更進行驗證的過程也很重要，可確保外部人員無法修改代碼而將惡意軟體引入系統。

## 9 Security Logging and Monitoring Failures 資安記錄及監控失效
- 之前名稱為記錄與監控不足風險，資安記錄及監控失效描述了入侵監控和report系統未能捕獲和寫入駭客入侵的跡象。
- 這可能是因為某些資安事件未記錄或日誌僅存儲在本地，或者警報值不足。
- 如果沒有足夠的report報告，數據洩露可能會在數月或數年內未被發現。

- 預防：為了防止資安記錄及監控不充分，資安管理員必須確認所有失敗的登錄嘗試和伺服器端輸入驗證都被立即記錄和警示。

## 10 Server-Side Request Forgery 伺服端請求偽造
- 伺服端請求偽造（SSRF）也是2021年新列入的。
- 當網頁應用程式正在取得遠端資源，卻未驗證由使用者提供的網址，此時就會發生偽造伺服端請求。
- 即便有防火牆、VPN或其他網路ACL保護的情況下，攻擊者仍得以強迫網頁應用程式發送一個經過捏造的請求給一個非預期的目的端。
- 這些損壞的請求可能會導致數據洩露。隨著雲端服務和雲端結構的複雜性，SSRF 攻擊的嚴重性將會愈來愈嚴峻。

- 預防：防止 SSRF 的最佳方法是配置網路訪問控制策略，實施預設“阻止所有外部流量”。
- 在應用上建議為用戶端提供的資料設置白名單允許列表。


![image](https://user-images.githubusercontent.com/71476327/195992362-65cbbad5-c12e-4f6a-8d10-70cb465a87cf.png)




