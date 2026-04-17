租屋資訊整合平台

系統需求規格書
Software Requirements Specification (SRS)
Version: 1.1

姓名 學號 E-mail
唐集憶 114598075 t114598075@ntut.org.tw
蔡秉宏 114598068 t114598068@ntut.org.tw
林鑫宏 114598038 t114598038@ntut.org.tw
王映儒 113598015 t113598015@ntut.org.tw

Department of Computer Science & Information Engineering
National Taipei University of Technology

04/17/2026

目錄 (Table of Contents)

目錄 (Table of Contents) i
Section 0 版次變更紀錄 (Change Log) 1
Section 1 簡介(Introduction) 2
1.1系統 (System) 2
1.1.1目標 (Purpose) 2
1.1.2系統名稱 (Identification) 2
1.1.3概觀 (Overview) 2
1.1.4控制文件 (Controlling Documents) 3
1.2文件 (Document) 3
1.2.1目的 (Purpose) 3
1.2.2驗收準則 (Acceptance Criteria) 3
1.2.3符號描述 (Notation Description) 3
1.2.4優先次序定義 (Priority Definition) 4
Section 2 系統(System) 5
2.1系統描述 (System Description) 5
2.1.1系統架構圖 (System Architecture Diagram) 5
2.2操作概念 (Operational Concepts) 5
2.3設計限制 (Design and Implementation Constrains) 5
2.4 技術限制 (Technological Limitations) 5
2.5介面需求 (Interface Requirements) 6
2.5.1使用者介面需求 (User Interfaces Requirements) 6
2.5.2外部介面需求 (External Interface Requirements) 6
2.5.3內部介面需求 (Internal Interface Requirements) 6
2.6功能性需求 (Functional Requirements) 6
2.6.1使用者故事與驗收準則 (User Stories and Acceptance Criteria) 7
2.7非功能性需求 (Non-Functional Requirements) 8
2.7.1效能需求 (Performance Requirements) 8
2.7.2資安需求 (Security Requirements) 8
2.7.3相容性需求 (Compatiability Requirements) 9
2.7.4測試需求 (Test Requirements) 9
2.8其他需求 (Other Requirements) 9
2.8.1環境需求 (Environmental Requirement) 9
2.8.2安裝需求 (Installation Requirement) 9
2.8.3交付需求 (Delivery Requirement) 9
2.8.4維護性需求 (Maintainability Requirements) 10
2.9追朔矩陣 (Traceability Matrix) 10
2.9.1需求對需求 (Requirements vs. Requirements) 10
2.9.2需求對使用者故事 (Requirements vs. User Stories) 11
2.9.3需求對模組 (Requirements vs. Modules) 11
2.9.4需求對介面 (Requirements vs. Interfaces) 12
Section 3 房源管理子系統 14
3.1 房源管理子系統描述 (LMS Description) 14
3.1.1系統架構圖 (System Context Diagram) 14
3.2 介面需求 (Interface Requirements) 14
3.2.1 使用者介面需求 (User Interfaces Requirements) 14
3.2.2 內部介面需求 (Internal Interface Requirements) 14
3.3 功能性需求 (Functional Requirements 14
3.4 非功能性需求 (Non-Functional Requirements) 15
3.4.1 效能需求 (Performance Requirements) 15
3.4.2 安全需求 (Security Requirements) 15
3.5 操作概念 (Operational Concepts) 15
3.6 設計限制 (Design Constraints) 15
Section 4 使用者身份驗證子系統 16
4.1 使用者身份驗證子系統描述 (UAS Description) 16
4.1.1系統架構圖 (System Context Diagram) 16
4.2 介面需求 (Interface Requirements) 16
4.2.1 使用者介面需求 (User Interfaces Requirements) 16
4.2.2 內部介面需求 (Internal Interface Requirements) 16
4.3 功能性需求 (Functional Requirements) 16
4.4 非功能性需求 (Non-Functional Requirements) 17
4.4.1 效能需求 (Performance Requirements) 17
4.4.2 安全需求 (Security Requirements) 17
4.5 其他需求 (Other Requirements) 17
4.5.1 測試需求 (Test Requirements) 17
4.6 操作概念 (Operational Concepts) 17
4.7 設計限制 (Design and Implementation Constraints) 18
Section 5 即時通訊子系統 19
5.1 即時通訊子系統描述 (Real-time Communication Subsystem Description) 19
5.1.1 系統架構圖 (System Context Diagram) 19
5.2 介面需求 (Interface Requirements) 19
5.2.1 使用者介面需求 (User Interfaces Requirements) 19
5.2.2 內部介面需求 (Internal Interface Requirements) 19
5.2.3 外部介面需求 (External Interface Requirements) 20
5.3 功能性需求 (Functional Requirements) 20
5.4 非功能性需求 (Non-Functional Requirements) 20
5.4.1 效能需求 (Performance Requirements) 20
5.4.2 安全需求 (Security Requirements) 20
5.5 其他需求 (Other Requirements) 20
5.5.1 維護性需求 (Maintainability Requirements) 20
5.5.2 安裝需求 (Installation Requirement) 20
5.6 操作概念 (Operational Concepts) 21
5.7 設計限制 (Design and Implementation Constraints) 21
Section 6 房源搜尋子系統 22
6.1 房源搜尋子系統描述（Listing Search Subsystem Description） 22
6.1.1 系統架構圖（System Context Diagram） 22
6.2 介面需求 (Interface Requirements) 22
6.2.1 外部介面需求（External Interface Requirements） 22
6.2.2 內部介面需求 (Internal Interface Requirements) 22
6.2.3 使用者介面需求（User Interface Requirements） 23
6.3 功能性需求（Functional Requirements） 23
6.4 效能需求（Performance Requirements） 23
6.5 測試需求（Test Requirements） 23
6.6 其他需求（Other Requirements） 23
6.7 操作概念（Operational Concepts） 24
6.8 設計限制（Design and Implementation Constraints） 24
Section 7 資料庫管理子系統 25
7.1 資料庫管理子系統描述 (DBMS Description) 25
7.1.1系統架構圖 (System Context Diagram) 25
7.2 介面需求 (Interface Requirements) 25
7.2.1 使用者介面需求 (User Interfaces Requirements) 25
7.2.2 內部介面需求 (Internal Interface Requirements) 25
7.3 功能性需求 (Functional Requirements) 25
7.4 非功能性需求 (Non-Functional Requirements) 26
7.4.1 效能需求 (Performance Requirements) 26
7.4.2 安全需求 (Security Requirements) 26
7.5 其他需求 (Other Requirements) 26
7.5.1 測試需求 (Test Requirements) 26
7.6 操作概念 (Operational Concepts) 26
7.7 設計限制 (Design and Implementation Constraints) 27
Glossary 28
References 29
Appendix 30

Section 0 版次變更紀錄 (Change Log)
Revisions
Verison Primary Author(s) Description of
Version Date Completed
1.0 唐集憶、蔡秉宏、林鑫宏、王映儒 SRS 規劃討論、大綱完成、簡介章節完成 2026/04/15
1.1 唐集憶、蔡秉宏、林鑫宏、王映儒 SRS 子系統章節完結 2026/04/17

 
Section 1 簡介(Introduction)
1.1系統 (System)
1.1.1目標 (Purpose)
在租屋市場中，租客與房東雙方皆面臨諸多困境。對租客而言，市面上的租屋資訊分散且缺乏透明度，潛藏詐騙風險，加上房租以外的管理費、押金、水電費、網路費等額外支出往往未於刊登頁面完整揭露，導致租客在尋屋過程中耗費大量時間與精力，卻仍難以找到符合需求的理想住所；對房東而言，傳統刊登管道觸及率有限，難以快速媒合合適租客，且傳統租屋聯繫方式多依賴電話進行同步即時溝通，需雙方同時在線且即時回應，缺乏時間彈性，亦不利於訊息保存與後續查詢。往往造成不必要的溝通成本與管理負擔。
有鑑於此，本平台旨在建立一個公開、透明且高效的線上租屋媒合環境，透過整合房源搜尋、即時通訊等核心功能，解決租客找屋困難與房東管理不便的痛點，並由平台管理員審核房源，進而提升整體租賃市場的效率與信任度。

1.1.2系統名稱 (Identification)
租屋資訊整合平台(Rental Information Aggregation Platform)，此系統包含的子系統為：

1. 房源管理子系統(Listing Management Subsystem)
2. 使用者身份驗證子系統(User Authentication Subsystem)
3. 即時通訊子系統(Real-time Communication Subsystem)
4. 房源搜尋子系統(Listing Search Subsystem)
5. 資料庫管理子系統(Database Management Subsystem)

1.1.3概觀 (Overview)
本系統共分為五個子系統：

1. 房源管理子系統(Listing Management Subsystem)
   負責處理房源從建立、上架到下架的完整生命週期。提供房東端刊登服務，強制要求完整揭露租金以外的附加費用（如押金、水電費、管理費等），以解決資訊不透明的問題。同時讓平台管理員能針對新上架的房源進行審核與查驗，手動過濾異常或詐騙房源，確保平台資訊的真實性與安全性。
2. 使用者身份驗證子系統(User Authentication Subsystem)
   負責系統的存取安全控制與會員身分管理。處理包含租客、房東及平台管理員的註冊、登入與登出作業。此子系統具備角色存取控制機制，確保不同身份的使用者僅能操作對應權限的功能。
3. 即時通訊子系統(Real-time Communication Subsystem)
   負責處理租客與房東之間的線上訊息傳遞。打破傳統依賴同步電話溝通的限制，提供非同步的文字訊息功能，讓雙方能在時間彈性的狀況下進行對話。此子系統會妥善保存歷史通訊紀錄，便於後續查詢與釐清細節，降低溝通成本並減少潛在糾紛。
4. 房源搜尋子系統(Listing Search Subsystem)
   負責提供租客端搜尋服務。整合多種搜尋條件、透明化的數據進行篩選，讓租客能過濾出符合自身需求的理想物件，解決市面上資訊分散且難以比對的找房痛點。
5. 資料庫管理子系統(Database Management Subsystem)
   負責作為系統核心邏輯與底層資料庫之間的資料存取介面。統一接收來自前述四個子系統（房源、驗證、通訊、搜尋）的存取請求，進行資料的格式驗證、讀寫（CRUD）與關聯運算，並將最終結果安全地寫入實體資料庫儲存層，以確保系統資料的完整性、一致性與安全性。

1.1.4控制文件 (Controlling Documents)
無

1.2文件 (Document)
1.2.1目的 (Purpose)
此文件目的為說明系統功能以及子系統功能需求,並且介紹各個系統之間的關聯,
作為系統開發者的溝通參考依據。

1.2.2驗收準則 (Acceptance Criteria)
● 明確且適當地陳述(Clearly and properly stated)
● 完整性(Completely)
● 一致性(Consistently)
● 能個別界定(Uniquely Identified)
● 能適當地執行(Appropriately implement)
● 能驗證(Verifiably)

1.2.3符號描述 (Notation Description)
Notation Description
RIAP Rental Information Aggregation Platform
LMS Listing Management Subsystem
UAS User Authentication Subsystem
RCS Real-time Communication Subsystem
LSS Listing Search Subsystem
DBMS Database Management Subsystem
DB Database

Notation Description
RIAP-F-nn RIAP Functional Requirements
RIAP-N-nn RIAP non-Functional Requirements
LMS-F-nn LMS Functional Requirements
LMS-N-nn LMS non-Functional Requirements
UAS-F-nn UAS Functional Requirements
UAS-N-nn UAS non-Functional Requirements
RCS-F-nn RCS Functional Requirements
RCS-N-nn RCS non-Functional Requirements
LSS-F-nn LSS Functional Requirements
LSS-N-nn LSS non-Functional Requirements
DBMS-F-nn DBMS Functional Requirements
DBMS-N-nn DBMS non-Functional Requirements

1.2.4優先次序定義 (Priority Definition)
NO. Name Description
1 Critical 此系統完成時必須具備的
2 Importance 系統完成可以不須立刻具備,但需在期限完成
3 Describe 此功能的加入可以改善各項功能,使其更便利
4 Optional 此為選擇性需求,不影響系統,亦可立為下次版本的參考

 
Section 2 系統(System)
2.1系統描述 (System Description)
2.1.1系統架構圖 (System Architecture Diagram)

圖2.1系統流程概念圖

2.2操作概念 (Operational Concepts)

1. 房客：可以搜尋房源、瀏覽房源明細、檢舉異常房源、並在帳號註冊與登入後可以發送/接收即時訊息
2. 房東：帳號註冊與登入後可以刊登/編輯房源、查看與回應房客即時訊息
3. 管理員：可以處理檢舉/違規封鎖、審核房源內容

2.3設計限制 (Design and Implementation Constrains)
需求編號 優先順序 需求描述
RIAP-N-01 1 程式、UI 及資料庫連結均採用 Java、JavaScript 撰寫設計。
RIAP-N-02 1 資料庫採用 PostgreSQL。

2.4 技術限制 (Technological Limitations)
需求編號 優先順序 需求描述
RIAP-N-03 1 使用者操作需基於 WEB 的 UI。
RIAP-N-04 1 因使用 PostgreSQL,需注意資料庫連線之安全性設定,以降低遭受入侵的危險。

2.5介面需求 (Interface Requirements)
2.5.1使用者介面需求 (User Interfaces Requirements)
需求編號 優先順序 需求描述
RIAP-N-05 1 系統登入介面。
RIAP-N-06 1 管理帳號介面。
RIAP-N-07 1 租房管理介面。
RIAP-N-08 1 搜尋房源介面。
RIAP-N-09 2 即時訊息介面

2.5.2外部介面需求 (External Interface Requirements)
需求編號 優先順序 需求描述
RIAP-N-10 1 DBMS 與實體 DB 伺服器間必須建立標準連線，以執行底層資料的儲存與檢索。
RIAP-N-11 1 系統所有與使用者介面之通訊必須透過標準傳輸協定 HTTPS，確保傳輸過程之安全性。
RIAP-N-12 1 系統必須能讀取使用者裝置之作業系統語系設定，以提供對應的語系介面。

2.5.3內部介面需求 (Internal Interface Requirements)
需求編號 優先順序 需求描述
RIAP-N-13 1 LMS、UAS、RCS 與 LSS 均必須透過 DBMS 進行資料存取，嚴禁直接跳過 DBMS 操作底層資料。
RIAP-N-14 1 DBMS 必須提供統一的 API 介面給各子系統，用以執行資料的 CRUD 運算。
RIAP-N-15 1 LMS 執行刊登操作前，必須向 UAS 請求目前使用者的 Session 狀態以驗證房東身分。
RIAP-N-16 1 RCS 啟動對話時，必須由 UAS 取得傳訊雙方的 UID 資訊，並由 LMS 取得對應房源的關聯 ID。
RIAP-N-17 1 LSS 執行房源篩選時，必須向 DBMS 請求包含費用明細在內的結構化欄位以進行計算。
RIAP-N-18 1 LMS 於房源狀態變更後，必須發送內部通知至 LSS 更新搜尋索引，確保房源狀態一致性。
RIAP-N-19 1 UAS 在偵測到異常登入或權限變更時，必須能主動通知 RCS 與 LMS 中斷該使用者的目前操作作業。

2.6功能性需求 (Functional Requirements)
需求編號 優先順序 需求描述
RIAP-F-01 1 身份驗證與帳號管理：系統需提供註冊、登入與登出功能。
RIAP-F-02 1 權限控管：系統需根據使用者身份（租客、房東、管理員）限制其可存取的介面與操作功能。
RIAP-F-03 1 房源刊登與編輯：房東可新增、修改房源資訊，包含標題、坪數、樓層及室內設備。
RIAP-F-04 1 費用強制揭露：房東刊登時，系統需強制要求填寫租金、押金、管理費、水電費計算基準。
RIAP-F-05 1 房源審核作業：管理員可對新上架房源進行核准或退回，未通過審核之物件不得公開顯示。
RIAP-F-06 1 多條件房源搜尋：租客可依地區、預算、坪數、房型及是否含特定雜費進行複合式篩選。
RIAP-F-07 2 關鍵字全文檢索：提供搜尋列，允許租客透過關鍵字搜尋標題與房源描述。
RIAP-F-08 1 即時通訊對話：租客可針對特定房源發送訊息給房東，房東可於系統內回覆。
RIAP-F-09 2 通訊紀錄保存：系統需儲存所有對話內容，供使用者隨時查閱歷史訊息。
RIAP-F-10 1 房源狀態同步：當房源成交或下架時，系統需即時更新資料庫並同步於搜尋結果中移除。

2.6.1使用者故事與驗收準則 (User Stories and Acceptance Criteria)
使用者故事：
需求編號 優先順序 使用者故事
RIAP-N-20 1 作為一名租客，我希望能透過預算和地區篩選房源，以便快速找到我負擔得起的房子。
RIAP-N-21 2 作為一名租客，我希望能直接在線上傳訊息給房東，而不必撥打電話，以節省溝通成本。
RIAP-N-22 1 作為一名房東，我希望能刊登我的房源資訊，並清晰列出租金、水電等各項費用，以減少資訊落差。
RIAP-N-23 1 作為一名房東，當我的房子租出去時，我希望能一鍵下架，避免持續收到詢問訊息。
RIAP-N-24 1 作為一名管理員，我希望能審核新刊登的物件，以過濾可能的詐騙或不實資訊，維護平台可信度。
RIAP-N-25 1 作為一名使用者，我希望能安全地登入系統，保護我的個人聯絡資訊與隱私。
RIAP-N-26 3 作為一名租客，我希望能檢舉資訊不實的房源，以提醒其他使用者注意風險。

驗收準則：
需求編號 優先順序 驗收準則
RIAP-F-11 1 1. 搜尋結果必須符合所選之地區與金額區間。2. 房源清單需能即時顯示包含管理費在內的總支出。
RIAP-F-12 2 1. 點擊聯絡房東應啟動即時通訊視窗。2. 雙方皆能檢視該訊息之傳送時間與內容紀錄。
RIAP-F-13 1 1. 刊登表單中，租金、押金與水電計算基準為必填欄位。2. 資料提交後，房源應處於「待審核」狀態而非立即公開。
RIAP-F-14 1 1. 房東切換狀態至「已租出」後，搜尋功能應立即過濾該物件。2. 原有的房源網頁應顯示「此物件已下架」。
RIAP-F-15 1 1. 管理員後台需能批次檢閱房源圖文內容。2. 若退回審核，系統需強制要求管理員輸入退回原因並通知房東。
RIAP-F-16 1 1. 登入時需經過密碼比對，錯誤達次數上限應暫時鎖定。2. 系統需根據身分導向至對應的功能選單。
RIAP-F-17 3 1. 房源頁面需提供檢舉按鈕。2. 提交檢舉後，管理員後台應能即時收到該物件的異常通報。

2.7非功能性需求 (Non-Functional Requirements)
需求編號 優先順序 需求描述
RIAP-N-27 1 系統頁面切換與載入時間必須小於 2 秒。
RIAP-N-28 1 執行房源篩選或關鍵字搜尋時，搜尋結果產生速度應小於 3 秒。
RIAP-N-29 2 即時訊息之傳送與接收延遲時間應小於 1 秒（在穩定網路環境下）。

2.7.1效能需求 (Performance Requirements)
需求編號 優先順序 需求描述
RIAP-N-30 1 必須通過針對 Use Case 所撰寫的 Test Case 測試。
RIAP-N-31 1 需針對身分驗證與權限控管進行單元測試 (Unit Test)，確保無權限越位問題。

2.7.2資安需求 (Security Requirements)
需求編號 優先順序 需求描述
RIAP-N-32 1 對使用者密碼進行加密儲存。
RIAP-N-33 1 系統開發需嚴格過濾使用者輸入，防止 SQL Injection 與 XSS (跨站腳本攻擊)。
RIAP-N-34 1 所有敏感資料傳輸必須強制使用 HTTPS 協定進行加密傳送。

2.7.3相容性需求 (Compatiability Requirements)
需求編號 優先順序 需求描述
RIAP-N-35 1 使用 RWD (響應式網頁設計)，使平台在電腦、平板與手機等不同尺寸裝置上均可正常顯示。
RIAP-N-36 2 系統需支援主流瀏覽器（如 Chrome、Firefox、Safari 及 Edge）之最新版本。

2.7.4測試需求 (Test Requirements)
需求編號 優先順序 需求描述
RIAP-N-37 1 必須通過針對 Use Case 所撰寫的 Test Case 測試。
RIAP-N-38 1 需針對身分驗證與權限控管進行單元測試 (Unit Test)，確保無權限越位問題。

2.8其他需求 (Other Requirements)
2.8.1環境需求 (Environmental Requirement)
需求編號 優先順序 需求描述
RIAP-N-39 1 伺服器主機需具備 Intel Core i5 2.5GHz 或同等級以上之處理器。
RIAP-N-40 1 伺服器可用記憶體 (RAM) 需至少 8GB 以上，以負荷併發之即時通訊請求。
RIAP-N-41 1 儲存空間 (Hard Disk) 需預留 1GB 以上供應用程式運行，房源圖片與資料庫空間另計。

2.8.2安裝需求 (Installation Requirement)
需求編號 優先順序 需求描述
RIAP-N-42 1 安裝並配置 PostgreSQL 13 以上版本之資料庫環境。
RIAP-N-43 1 執行資料庫初始化腳本，建立所有必要之資料表、索引與關聯鍵。
RIAP-N-44 1 安裝 Java Runtime Environment (JRE) 或 JDK 17 以上版本以執行系統後端。

2.8.3交付需求 (Delivery Requirement)
需求編號 優先順序 需求描述
RIAP-N-45 1 交付之軟體成品必須完全符合本 RIAP 系統需求規格書之定義。
RIAP-N-46 1 需交付完整程式原始碼、資料庫架構圖、以及系統操作手冊。

2.8.4維護性需求 (Maintainability Requirements)
需求編號 優先順序 需求描述
RIAP-N-47 1 由開發團隊提供後續系統維護與技術支援。
RIAP-N-48 2 程式碼需具備詳細註解並符合 Java 命名規範，以利後續功能擴充與除錯。

2.9追朔矩陣 (Traceability Matrix)
2.9.1需求對需求 (Requirements vs. Requirements)
RIAP-F-11 RIAP-F-12 RIAP-F-13 RIAP-F-14 RIAP-F-15 RIAP-F-16 RIAP-F-17 RIAP-F-27 RIAP-F-28 RIAP-F-29 RIAP-F-30 RIAP-F-31 RIAP-F-32 RIAP-F-33 RIAP-F-34
RIAP-F-01 　 　 　 　 　 V 　 V 　 　 V V V V V
RIAP-F-02 　 　 　 　 V V V V 　 　 V V 　 　 　
RIAP-F-03 　 　 V 　 　 　 　 V 　 　 V 　 　 V 　
RIAP-F-04 　 V 　 　 　 　 　 　 　 V 　 　 V 　
RIAP-F-05 　 　 V 　 V 　 　 V 　 　 V 　 　 　 　
RIAP-F-06 V 　 　 V 　 　 　 V V 　 V 　 　 V 　
RIAP-F-07 　 　 　 　 　 　 　 　 V 　 V 　 　 V 　
RIAP-F-08 　 V 　 　 　 　 　 V 　 V V 　 　 V V
RIAP-F-09 　 V 　 　 　 　 　 　 　 　 V 　 　 　 　
RIAP-F-10 　 　 　 V 　 　 　 V 　 　 V 　 　 　 　

2.9.2需求對使用者故事 (Requirements vs. User Stories)
RIAP-F-01 RIAP-F-02 RIAP-F-03 RIAP-F-04 RIAP-F-05 RIAP-F-06 RIAP-F-07 RIAP-F-08 RIAP-F-09 RIAP-F-10
RIAP-N-20 V V
RIAP-N-21 V V V V
RIAP-N-22 V V V V V
RIAP-N-23 V V V V
RIAP-N-24 V V V
RIAP-N-25 V V
RIAP-N-26 V V

2.9.3需求對模組 (Requirements vs. Modules)
LMS UAS RCS LSS DMS
RIAP-F-01 V V
RIAP-F-02 V V
RIAP-F-03 V V V
RIAP-F-04 V V V
RIAP-F-05 V V V V
RIAP-F-06 V V
RIAP-F-07 V V
RIAP-F-08 V V V
RIAP-F-09 V V V
RIAP-F-10 V V V

2.9.4需求對介面 (Requirements vs. Interfaces)
RIAP-N-5 RIAP-N-6 RIAP-N-7 RIAP-N-8 RIAP-N-9 RIAP-N-10 RIAP-N-11 RIAP-N-12 RIAP-N-13 RIAP-N-14 RIAP-N-15 RIAP-N-16 RIAP-N-17 RIAP-N-18 RIAP-N-19
RIAP-F-01 V 　 　 　 　 V V V V V 　 　 　 　 V
RIAP-F-02 V V 　 　 　 V V V V V 　 　 　 　 V
RIAP-F-03 　 　 V 　 　 V V V V V V 　 　 　 　
RIAP-F-04 　 　 V 　 　 V V V V V 　 　 V 　 　
RIAP-F-05 　 V 　 　 　 V V V V V 　 　 　 　 　
RIAP-F-06 　 　 　 V 　 V V V V V 　 　 V 　 　
RIAP-F-07 　 　 　 V 　 V V V V V 　 　 　 V 　
RIAP-F-08 　 　 　 　 V V V V V V 　 V 　 　 　
RIAP-F-09 　 　 　 　 V V V V V V 　 　 　 　 　
RIAP-F-10 　 　 V V 　 V V V V V 　 　 　 V 　

 
Section 3 房源管理子系統
3.1 房源管理子系統描述 (LMS Description)
房源管理子系統（LMS）負責處理平台內房源從建立、上架、內容變更至下架的完整生命週期 。本子系統的核心目標在於解決租屋市場資訊不透明的痛點，透過強制性的費用公布機制（如押金、水電費、管理費等），確保租客獲取真實且完整的資訊 。此外，本子系統亦包含管理端審核流程，由平台管理員手動過濾異常或詐騙房源，以維護平台的資訊安全與可信度 。

3.1.1系統架構圖 (System Context Diagram)

圖3.1.1 系統架構圖

3.2 介面需求 (Interface Requirements)
3.2.1 使用者介面需求 (User Interfaces Requirements)
需求編號 優先順序 需求描述
LMS-N-01 1 房源刊登介面：提供房東輸入房源標題、坪數、樓層、室內設備及強制性費用明細。
LMS-N-02 1 房源編輯介面：允許房東修改已上架或待審核的房源內容。
LMS-N-03 1 管理員審核介面：提供平台管理員批次檢閱房源圖文，並執行核准或退回操作。
LMS-N-04 1 房源狀態管理介面：提供房東「一鍵下架」或切換為「已租出」狀態的功能。

3.2.2 內部介面需求 (Internal Interface Requirements)
需求編號 優先順序 需求描述
LMS-N-05 1 LMS 必須透過 DBMS進行資料存取，嚴禁直接操作底層資料庫。
LMS-N-06 1 LMS 執行刊登操作前，必須向 UAS 請求目前使用者的 Session 狀態以驗證房東身份。
LMS-N-07 1 LMS 於房源狀態變更（如成交或下架）後，必須通知 LSS 更新搜尋索引。
LMS-N-08 1 當 RCS 啟動對話時，LMS 必須提供對應房源的關聯 ID 與基本資訊。

3.3 功能性需求 (Functional Requirements
需求編號 優先順序 需求描述
LMS-F-01 1 房源資訊建立：房東可新增房源，包含標題、坪數、樓層及設備資訊 。
LMS-F-02 1 費用公開透明：系統強制房東填寫租金、押金、管理費及水電費計算基準，否則不予提交 。
LMS-F-03 1 審核工作流：新刊登房源預設為「待審核」狀態，需經管理員核准後方可公開顯示 。
LMS-F-04 1 退回通知機制：房源若被退回，系統需強制管理員輸入原因並通知房東 。
LMS-F-05 1 狀態同步更新：房源狀態變更需即時同步至資料庫，並反映於搜尋結果中 。

3.4 非功能性需求 (Non-Functional Requirements)
3.4.1 效能需求 (Performance Requirements)
需求編號 優先順序 需求描述
LMS-N-09 1 效能要求：房源圖片上傳與表單提交之系統回應時間應小於 3 秒 。

3.4.2 安全需求 (Security Requirements)
需求編號 優先順序 需求描述
LMS-N-10 1 安全性：房東僅能編輯或下架屬於自己 UID 關聯之房源資訊 。
LMS-N-11 1 資料完整性：所有輸入欄位需進行伺服器端驗證，防止不合法的資料寫入資料庫 。

3.5 操作概念 (Operational Concepts)

1. 房源刊登流程：房東經由 UAS 登入後，進入 LMS 刊登頁面，填寫包含費用在內的完整資訊。提交後，系統將資料寫入資料庫並標記為「待審核」 。
2. 審核流程：管理員於後台查閱待審核列表。核准後，LMS 發送通知至 LSS 更新索引使房源公開；若退回，則記錄原因並要求房東修正 。
3. 結案下架：當房源租出，房東於介面執行下架，LMS 即時更新 DB 狀態，確保搜尋結果中不再出現該物件 。

3.6 設計限制 (Design Constraints)
需求編號 優先順序 需求描述
LMS-N-12 1 開發語言：必須採用 Java 與 JavaScript 進行撰寫與設計 。
LMS-N-13 1 資料庫：所有房源資料必須儲存於 PostgreSQL 資料庫 。
LMS-N-14 1 通訊協定：所有與使用者介面之通訊必須透過 HTTPS 確保安全 。
Section 4 使用者身份驗證子系統
4.1 使用者身份驗證子系統描述 (UAS Description)
使用者身份驗證子系統（UAS）負責系統的存取安全控制與會員身分管理。本子系統主要處理包含租客、房東及平台管理員的註冊、登入與登出作業。此外，此子系統具備嚴密的角色存取控制機制（Role-Based Access Control），可確保不同身份的使用者僅能存取與操作其對應權限的功能，以保障平台整體資訊安全與隱私。

4.1.1系統架構圖 (System Context Diagram)

4.2 介面需求 (Interface Requirements)
4.2.1 使用者介面需求 (User Interfaces Requirements)
需求編號 優先順序 需求描述
UAS-N-01 1 系統登入與註冊介面：提供使用者輸入帳號、密碼進行登入，以及新使用者選擇身份（租客/房東）進行註冊的表單介面 。
UAS-N-02 1 密碼重置介面：提供使用者在忘記密碼時，輸入驗證資訊以重置密碼的頁面。
UAS-N-03 1 權限阻擋提示介面：當使用者嘗試越權存取非其身份可操作之頁面時，顯示「無權限訪問」之提示與導航介面。

4.2.2 內部介面需求 (Internal Interface Requirements)
需求編號 優先順序 需求描述
UAS-N-04 1 UAS 必須透過 DBMS 進行會員資料之存取與驗證，嚴禁直接跳過 DBMS 操作底層資料 。
UAS-N-05 1 LMS 執行刊登等操作前，UAS 必須能接收並回應其對於目前使用者 Session 狀態與房東身分的驗證請求 。
UAS-N-06 1 當 RCS 啟動對話時，UAS 必須負責提供傳訊雙方的 UID 資訊給 RCS 系統 。
UAS-N-07 1 UAS 在偵測到異常登入或權限變更時，必須能主動通知 RCS 與 LMS 中斷該使用者的目前操作作業 。

4.3 功能性需求 (Functional Requirements)
需求編號 優先順序 需求描述
UAS-F-01 1 身份驗證與帳號管理：系統需提供租客、房東及管理員的註冊、登入與登出功能 。
UAS-F-02 1 權限控管：系統需根據登入之使用者身份（租客、房東、管理員），限制其可存取的介面與操作功能 。
UAS-F-03 1 功能導向：系統需於使用者成功登入後，根據其身分自動導向至對應的專屬功能選單或後台 。
UAS-F-04 1 異常登入防範：登入時需經過密碼比對，若密碼輸入錯誤達系統設定之次數上限，應暫時鎖定該帳號以防暴力破解 。
4.4 非功能性需求 (Non-Functional Requirements)

4.4.1 效能需求 (Performance Requirements)
需求編號 優先順序 需求描述
UAS-N-08 1 身份驗證與登入請求之處理回應時間，在穩定網路環境下必須小於 2 秒。

4.4.2 安全需求 (Security Requirements)
需求編號 優先順序 需求描述
UAS-N-09 1 密碼保護：系統必須對使用者的登入密碼進行單向雜湊加密（如 Bcrypt 或 Argon2）儲存，嚴禁以明碼存放於資料庫中 。
UAS-N-10 1 傳輸安全：所有涉及身分驗證與帳號密碼的敏感資料傳輸，必須強制使用 HTTPS 協定進行加密傳送 。
UAS-N-11 1 安全防護：登入與註冊表單需嚴格過濾使用者輸入，防止 SQL Injection 與 XSS (跨站腳本攻擊) 。

4.5 其他需求 (Other Requirements)
4.5.1 測試需求 (Test Requirements)
需求編號 優先順序 需求描述
UAS-N-12 1 必須針對身分驗證（Authentication）與權限控管（Authorization）進行單元測試 (Unit Test)，確保無權限越位問題 。
UAS-N-13 1 系統需安全地保護使用者的個人聯絡資訊與隱私，並通過對應之資安測試案例 。

4.6 操作概念 (Operational Concepts)

1. 註冊與登入流程：使用者透過系統首頁進入登入/註冊介面。若為新使用者，需選擇「租客」或「房東」身分並填寫必要資訊；既有使用者則輸入帳密。UAS 接收請求後，透過 DBMS 向資料庫驗證憑證，成功後發放 Session 或 Token，並根據身分導向相應首頁。
2. 跨子系統權限驗證：當使用者在平台內進行任何受限操作（例如：房東嘗試進入 LMS 編輯房源、租客嘗試進入 RCS 發送訊息），各子系統（LMS/RCS）皆會在後台向 UAS 請求驗證目前的 Session 狀態。若 UAS 回報未登入或權限不符，則即時阻擋該次操作並要求重新登入。
3. 登出與工作階段終止：使用者主動點擊登出，或 UAS 偵測到異常、閒置逾時，UAS 會立即銷毀該工作階段（Session/Token），並通知其他子系統中斷關聯操作。

4.7 設計限制 (Design and Implementation Constraints)
需求編號 優先順序 需求描述
UAS-N-14 1 驗證邏輯與資料存取必須分離，UAS 不得直接操作 PostgreSQL，必須統一透過 DBMS 提供的介面執行查詢 。
UAS-N-15 1 後端驗證機制需以 Java 開發，並符合平台整體的模組化架構規範 。

 
Section 5 即時通訊子系統
5.1 即時通訊子系統描述 (Real-time Communication Subsystem Description)
即時通訊子系統 (RCS) 旨在打破租客與房東之間傳統電話溝通的限制，提供一個非同步且具備紀錄留存功能的線上對話平台。
主要功能包含建立對話視窗、傳送文字訊息、檢視歷史訊息紀錄以及訊息讀取狀態顯示。

5.1.1 系統架構圖 (System Context Diagram)

圖5.1.1 系統架構圖

5.2 介面需求 (Interface Requirements)
5.2.1 使用者介面需求 (User Interfaces Requirements)
需求編號 優先順序 需求描述
RCS-N-01 1 對話列表介面：顯示使用者目前所有參與的對話，並提示未讀訊息數量。
RCS-N-02 1 即時聊天視窗：提供文字輸入、歷史訊息顯示與對象基本資料連結。
RCS-N-03 2 推播通知介面：在瀏覽器或作業系統視窗顯示新訊息提醒。

5.2.2 內部介面需求 (Internal Interface Requirements)
需求編號 優先順序 需求描述
RCS-N-04 1 RCS 必須向 UAS 請求目前使用者的 Session 與 UID，以識別訊息傳送者身分。
RCS-N-05 1 RCS 必須透過 DBMS 將每一則訊息持久化儲存至 PostgreSQL 資料庫中。
RCS-N-06 1 RCS 必須從 LMS 獲取房源基本資訊（如縮圖、標題），用於顯示對話關聯的物件資訊。
5.2.3 外部介面需求 (External Interface Requirements)
需求編號 優先順序 需求描述
RCS-N-07 1 訊息傳輸必須基於 WebSocket 或同等即時協定，並強制使用 HTTPS/WSS 加密。

5.3 功能性需求 (Functional Requirements)
需求編號 優先順序 需求描述
RCS-F-01 1 發送訊息：使用者可輸入文字訊息並即時傳送給對象。
RCS-F-02 1 接收訊息：系統需在不重新整理頁面的情況下，即時更新對話內容。
RCS-F-03 1 歷史紀錄存取：當使用者進入對話時，系統需自動載入該對話之歷史訊息。
RCS-F-04 2 已讀狀態顯示：系統需顯示訊息是否已被對方閱讀。
RCS-F-05 2 房源關聯建立：當租客從房源頁面發起對話時，系統需自動帶入該房源 ID。

5.4 非功能性需求 (Non-Functional Requirements)
5.4.1 效能需求 (Performance Requirements)
需求編號 優先順序 需求描述
RCS-N-08 1 訊息傳遞延遲時間（從傳送至對方收到）在網路正常情況下應小於 1 秒。
RCS-N-09 2 歷史訊息載入（前 20 則）應在 1.5 秒內完成。

5.4.2 安全需求 (Security Requirements)
需求編號 優先順序 需求描述
RCS-N-10 1 系統須確保使用者無法透過修改參數來讀取非本人參與之對話紀錄。
RCS-N-11 1 對訊息輸入內容進行過濾（Sanitization），防止儲存型 XSS 攻擊。

5.5 其他需求 (Other Requirements)
5.5.1 維護性需求 (Maintainability Requirements)
需求編號 優先順序 需求描述
RCS-N-12 1 由程式開發者提供即時通訊模組之 API 說明文件。

5.5.2 安裝需求 (Installation Requirement)
需求編號 優先順序 需求描述
RCS-N-13 1 資料庫需建立 messages 與 chat_sessions 之關聯資料表。
5.6 操作概念 (Operational Concepts)
啟動對話：租客在瀏覽 LMS 提供的房源頁面時，點擊「聯絡房東」，RCS 將向 UAS 確認租客身分，並在 chat_sessions 建立一條關聯該房源 ID 的紀錄。
即時互動：雙方進入聊天室後，瀏覽器透過 WebSocket 與 RCS 伺服器保持連線，實現雙向即時通訊。
訊息持久化：每當有一則新訊息產生，RCS 會先呼叫 DBMS 寫入資料庫，確保使用者下次登入時仍可查詢歷史紀錄。

5.7 設計限制 (Design and Implementation Constraints)
需求編號 優先順序 需求描述
RCS-N-14 1 即時通訊後端建議採用 Socket.io 或 Java WebSocket API 實現。
RCS-N-15 1 每一則文字訊息上限為 1000 個字元。

 
Section 6 房源搜尋子系統
6.1 房源搜尋子系統描述（Listing Search Subsystem Description）
讓使用者能透過條件篩選快速找到符合需求的房源資訊。使用者可依據地區、租金範圍、房型、設備條件（如是否有網路、家具、冷氣等）進行篩選，系統會即時從資料庫中查詢符合條件的房源，並以列表方式回傳給前端介面。

6.1.1 系統架構圖（System Context Diagram）

6.2 介面需求 (Interface Requirements)
6.2.1 外部介面需求（External Interface Requirements）
需求編號 優先順序 需求描述
LSS-N-01 1 LSS 必須能透過 DBMS 存取房源相關資料
LSS-N-02 1 Tenant Interface 可透過 HTTP/HTTPS 向 LSS 發送搜尋請求
LSS-N-03 1 LSS 回傳資料需支援 JSON 格式以供前端解析
LSS-N-04 1 系統需支援跨模組（UAS 驗證後）之查詢請求

6.2.2 內部介面需求 (Internal Interface Requirements)
需求編號 優先順序 需求描述
LSS-N-05 1 LSS 必須能從 DBMS 讀取房源資料但不得直接修改資料庫
LSS-N-06 1 LSS 必須支援多條件查詢（地區、價格區間、設備條件）
LSS-N-07 1 LSS 與 DBMS 之間需使用標準化 API 或 DAO 介面
LSS-N-08 1 查詢結果需統一格式化後回傳給前端或 API Gateway
LSS-N-09 2 LSS 必須支援快取機制以提升查詢效率

6.2.3 使用者介面需求（User Interface Requirements）
需求編號 優先順序 需求描述
LSS-N-10 1 提供搜尋頁面讓使用者輸入地區與租金範圍
LSS-N-11 1 提供篩選選項（如：是否有網路、是否可養寵物、是否含家具）
LSS-N-12 1 顯示房源列表（圖片、價格、地點、簡述）
LSS-N-13 2 提供排序功能（價格低→高、最新刊登）
LSS-N-14 1 點擊房源可進入詳細資訊頁面

6.3 功能性需求（Functional Requirements）
需求編號 優先順序 需求描述
LSS-F-01 1 系統需支援租金區間篩選（最低價～最高價）
LSS-F-02 1 系統需支援地區條件篩選（台北市、新北市等）
LSS-F-03 1 系統需支援設備條件篩選（網路、家具、冷氣等）
LSS-F-04 1 系統需支援房型條件篩選（套房、雅房、整層）
LSS-F-05 1 系統需能回傳符合條件之房源列表
LSS-F-06 2 系統需支援排序功能（價格、時間）

6.4 效能需求（Performance Requirements）
需求編號 優先順序 需求描述
LSS-N-15 1 一般查詢回應時間需小於 2 秒
LSS-N-16 1 高負載情況下查詢回應時間需小於 3 秒
LSS-N-17 1 系統需支援至少每秒 50 次查詢請求
LSS-N-18 1 搜尋結果列表載入時間需小於 1.5 秒
LSS-N-19 2 系統需支援快取以減少 DB 查詢負載

6.5 測試需求（Test Requirements）
需求編號 優先順序 需求描述
LSS-N-20 1 必須通過各種搜尋條件組合之測試案例
LSS-N-21 1 必須驗證租金範圍查詢正確性
LSS-N-22 1 必須驗證地區篩選結果正確性
LSS-N-23 1 必須測試多條件交集查詢（AND / OR 條件）
LSS-N-24 1 必須符合功能性與非功能性需求測試標準

6.6 其他需求（Other Requirements）
需求編號 優先順序 需求描述
LSS-F-07 1 系統需支援未來擴充更多篩選條件（如捷運距離）
LSS-F-08 1 系統需支援多語系擴充
LSS-N-25 2 系統需具備基本錯誤處理機制（查無資料回傳提示）
LSS-N-26 2 系統需具備日誌記錄查詢行為（log tracking）
LSS-N-27 1 系統需符合基本資安要求（避免 SQL Injection）

6.7 操作概念（Operational Concepts）
需求編號 優先順序 需求描述
LSS-N-28 1 使用者進入租屋平台搜尋頁面
LSS-N-29 1 輸入條件（地區、租金、設備需求等）
LSS-N-30 1 系統送出查詢請求至 LSS
LSS-N-31 1 LSS 向 DBMS 查詢符合條件之房源資料
LSS-N-32 1 DBMS 從DB結果並回傳
LSS-N-33 1 系統將結果整理後以列表方式呈現給使用者
LSS-N-34 1 使用者可進一步點擊房源查看詳細資訊

6.8 設計限制（Design and Implementation Constraints）
需求編號 優先順序 需求描述
LSS-N-35 1 資料庫需使用 PostgreSQL作為主要儲存系統
LSS-N-36 1 後端需符合 RIAP 模組化架構（LMS / UAS / RCS / LSS）
LSS-N-37 1 LSS 不可直接存取 DB，需透過 DBMS
LSS-N-38 1 API 傳輸格式需使用 JSON
LSS-N-39 1 系統需支援 RESTful API 設計
LSS-N-40 1 必須遵守基本 MVC 架構或分層式架構設計

 
Section 7資料庫管理子系統
7.1 資料庫管理子系統描述 (DBMS Description)
資料庫管理子系統（DBMS）是本平台的資料核心，負責統一管理所有結構化資料的儲存、查詢、更新與刪除作業。其目標是確保資料的完整性（Integrity）、安全性與高可用性。DBMS 封裝了底層資料庫（PostgreSQL）的操作邏輯，並為「使用者身份驗證 (UAS)」、「房源管理 (LMS)」、「租屋通訊 (RCS)」與「房源搜尋 (LSS)」等子系統提供標準化的資料存取介面，以落實系統解耦（Decoupling）。

7.1.1系統架構圖 (System Context Diagram)

7.2 介面需求 (Interface Requirements)
7.2.1 使用者介面需求 (User Interfaces Requirements)
需求編號 優先順序 需求描述
DBMS-N-01 2 資料管理後台介面：僅限平台管理員使用，提供直觀的介面以進行資料備份啟動、日誌查看及異常資料修復。

7.2.2 內部介面需求 (Internal Interface Requirements)
需求編號 優先順序 需求描述
DBMS-N-02 1 通用查詢介面：需提供標準化的 SQL 封裝介面（如 DAO 或 Repository），供 UAS、LMS、RCS、LSS 進行資料交換。
DBMS-N-03 1 交易控管介面：提供事務（Transaction）管理機制，確保涉及多表操作時（如預約房源並發送訊息）的資料一致性。
DBMS-N-04 1 連線池管理介面：系統需管理與 PostgreSQL 的連線數量，避免因過多併發連線導致效能崩潰。

7.3 功能性需求 (Functional Requirements)
需求編號 優先順序 需求描述
DBMS-F-01 1 資料持久化：系統需完整儲存使用者資料、房源細節、圖片路徑、對話紀錄及系統日誌。
DBMS-F-02 1 CRUD 基礎操作：支援所有業務子系統對資料庫進行的新增、讀取、更新與刪除請求。
DBMS-F-03 1 資料完整性約束：透過外鍵（Foreign Key）與 Check 約束，確保如「房源必須歸屬於存在之房東」等邏輯成立。
DBMS-F-04 2 自動備份功能：系統需支援定期（如每日凌晨）將資料庫內容備份至指定路徑或雲端儲存空間。

7.4 非功能性需求 (Non-Functional Requirements)
7.4.1 效能需求 (Performance Requirements)
需求編號 優先順序 需求描述
DBMS-N-05 1 高併發支援：在至少 50 人同時進行複雜查詢時，資料庫回應時間（Latency）應維持在 500ms 以內。
DBMS-N-06 1 索引優化：針對 LSS 常用之篩選欄位（如地區、租金、房型）建立 Index，優化查詢效率。

7.4.2 安全需求 (Security Requirements)
需求編號 優先順序 需求描述
DBMS-N-07 1 存取控制：資料庫僅接受來自應用伺服器（Application Server）的內部連線，嚴禁直接開啟對外（Public）之存取埠。
DBMS-N-08 1 ACID 特性：系統需完全符合原子性、一致性、隔離性、持久性，防止因系統當機導致資料遺失或損壞。
DBMS-N-09 2 資料恢復能力：若發生災難性故障，系統需能在 2 小時內從備份檔案恢復至最後一次成功備份的狀態。

7.5 其他需求 (Other Requirements)
7.5.1 測試需求 (Test Requirements)
需求編號 優先順序 需求描述
DBMS-N-10 1 執行壓力測試，模擬多個子系統同時請求大批量資料，驗證連線池與鎖定（Locking）機制之穩定性。
DBMS-N-11 1 進行資料一致性測試，驗證刪除父資料（如刪除房東帳號）時，相關聯資料（如其房源）是否能正確處理（級聯刪除或限制）。

7.6 操作概念 (Operational Concepts)

1. 資料存取流程：當 LMS 子系統需要刊登新房源時，會呼叫 DBMS 提供的 saveListing() 介面。DBMS 驗證資料格式後，將資料寫入 PostgreSQL 的對應資料表，並返回操作成功之 ID 給 LMS。
2. 搜尋優化機制：為了配合 LSS 的高效搜尋，DBMS 會維護多個複合索引，並定期執行 ANALYZE 指令以更新查詢優化器的統計資訊，確保搜尋效能不隨資料量增加而線性衰退。
3. 備份與監控：DBMS 會在背景執行健康監控。若偵測到磁碟空間不足或連線逾時，將自動記錄於系統日誌，並通知管理員。

7.7 設計限制 (Design and Implementation Constraints)
需求編號 優先順序 需求描述
DBMS-N-12 1 資料庫選型：必須使用 PostgreSQL 作為主要的關聯式資料庫系統。
DBMS-N-13 1 ORM 使用規範：開發時建議使用 Hibernate 或 JPA 進行物件關聯映射，以確保程式碼的可讀性與可維護性。

 
Glossary
術語 定義與描述
PostgreSQL 本系統採用的主要關聯式資料庫系統 ，要求版本需在 16及以上。
Java 後端開發與驗證機制所使用的程式語言 ，需使用 JDK 17 及以上版本。
JavaScript UI 與資料庫連結撰寫設計所採用的程式語言。
HTTPS 系統所有與使用者介面之通訊必須透過此標準傳輸協定，以確保安全性。
WebSocket / WSS 即時通訊子系統 (RCS) 訊息傳輸所基於的即時通訊協定。
CRUD 代表資料的新增 (Create)、讀取 (Read)、更新 (Update) 與刪除 (Delete) 等基礎運算。
RWD 響應式網頁設計 (Responsive Web Design)：確保平台在不同尺寸裝置（如電腦、平板、手機）上均可正常顯示。
SQL Injection / XSS 系統需嚴格過濾輸入以防範的常見資安攻擊手段，包含 SQL 注入與跨站腳本攻擊。
API 應用程式介面：由 DBMS 提供給各子系統執行資料存取之統一標準介面。
ORM 物件關聯映射：建議使用 Hibernate 或 JPA 進行開發，以確保程式碼的可讀性與可維護性。
ACID 資料庫必須符合的特性：原子性、一致性、隔離性、持久性，防止因故障導致資料遺失。

 
References

 
Appendix
