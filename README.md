###### tags: `job`

# Interview logs

### TOC
* [Tagtoo科技跨平台網路廣告](#tagtoo-科技跨平台網路廣告)
* [趨勢科技TrendMicro](趨勢科技-trendmicro)

### Tagtoo科技跨平台網路廣告
* job: 後端工程師
* interviewer: Teddy
* location: 臺北市信義路四段267號11F
* date: 2018.12.20
* questions:
    1. 有沒有用Django開發過什麼專案？
    2. 有用過GCP的什麼服務？有用過GKE嗎？
    3. 看你的經歷，為什麼又想回業界？
    4. 有沒有AI的經驗？用過什麼工具（視覺化、統計分析）？
    5. 為什麼會想投我們公司？是哪個部份吸引你？
* answers:
    1. 以我在目前任職的農科院有開發過的兩個專案來回答
    2. 主要是使用compute engine，有舉出使用情境：為了幫公司測試tableau server的功能，分別在GCP部署了tableau server及api server；另外有補充是以docker來做部署；至於GKE的部份還沒有摸過
    3. 這個問題我說明了在業界的公司為什麼離職，之後又為什麼會找公部門的工作，有點可惜沒回答到重點，其實主要是業界的技術水準跟real world的營運，能學到更多的東西，另外一方面則是薪水
    4. 回答之前線上課程有上過相關課程，用numpy、pandas、seaborn來打kaggle的經驗
    5. 這一題回答得不好，我回答因為公司所使用的技術滿吸引我，但沒有表現出對廣告投放或資料分析這方面的興趣
* information:
    - 目前Tagtoo的廣告拓及率已是領導的地位、規模也在擴張（東南亞：馬來西亞、印尼等），之前比較沒有用AI技術來分析資料（2-3億筆cookie），現在逐漸在加強這方面的分析應用
    - 不接受遠端工作，老闆覺得見面的直接溝通最有效率
    - 應徵的信件應該都是老闆自己回覆的
* references:
    - [四年後的你會在哪裡？─ Tagtoo 的創業故事](http://mrjamie.cc/2013/12/05/tagtoo/)
    - [我的新鮮人面試紀錄](https://blog.m157q.tw/posts/2016/02/12/first-job-interviews/)
    - [我的新鮮人離職紀錄](https://blog.m157q.tw/posts/2017/12/26/i-left-my-first-full-time-job/)


### 趨勢科技TrendMicro
* job: QA@Consumer Segment
* interviewer: Catherine、John
* location: 台北市大安區敦化南路二段198號8F
* date: 2018.12.21
* questions:
    - 一面
        1. 介紹你最近全端開發的專案？
        2. 你說的這個專案是部署在哪裡？為什麼不部署在雲端？
        3. 你的專案有寫過任何測試嗎？是什麼樣的測試？
        4. 為什麼你會針對穩定性來做測試？
        5. 你的專案主要用到什麼工具？
        6. 你之前在業界任職時的專案開發流程為何？
        7. 你的優點跟缺點為何？
        8. 請排序你最想當的角色：code、maintain、testing、design
    - 二面
        1. 為什麼考卷最後一題是送分題你卻沒寫到？是時間太短嗎？
        2. 如果今天桌上有5顆外觀一模一樣的球，但重量不同，給你1個磅秤，你能在幾次比較過後依重量完成排序？
        3. 同上題，如果今天已知其中3顆球和其中2顆球重量相同，能減少你比較的次數嗎？
        4. 如果9跟3的交集是1，聯集是多少？
        5. 今天讓你測試一個登入頁面，有email、password跟1個登入按鈕，你會怎麼測試？
        6. 為什麼前兩個工作性質差異這麼大？
        7. 你有什麼壞習慣？
        8. 人生遇過最大的困難是什麼？
        9. 你守時嗎？
        10. 你未來短、中、長期計畫是什麼？
* answers:
    - 一面
        1. 介紹了我用Django開發的視覺化網站，專案的緣由以及要解決什麼問題
        2. 部屬在Local Windows Server上，說明因為專案性質跟資源因此沒有部署在雲端，有說明其中利弊
        3. 這個專案從多個API抓取資料，有測試抓取資料的函式及紀錄log，另外針對執行時段較長（如時間範圍廣的）有另外測試
        4. 這個問題一時想不出來怎麼回答，就回答了因為遇到某個問題必須加上這樣的測試
        5. 抓取資料的排程用了redis、celery，後端是django，前端主要用到highchart.js及datatable.js
        6. 一個junior做開發，自訂合理的開發時程或senior同意後開始開發，其中有遇到問題適時反應給senior知道，pm對整個專案的成果負責
        7. 說明了太過悲觀主義，有時想太多劃地自限，但這同時是個優點也是個缺點
        8. code > mantain > testing > design
    - 二面
        1. 答題時間沒有規劃好，不應該發生這樣的事
        2. 磅秤是一種比較排序法，最佳時間複雜度會是O(NlogN)
        3. 答不出來，但可能可以減少？
        4. 原本超簡單的題目一時竟然回答不出來，腦袋卡在為什麼9跟3交集會是1，其中是經過什麼運算得到?主管回覆說可以，但不用想這麼複雜有直接答案
        5. 測試form沒填正確回覆的錯誤訊息是否正確，改變cookie來測試session，之後主管補充可以抓背後的API測試
        6. 這題回答得太長，但主要是遇到突發狀況跟想轉語言
        7. 有強迫症動作、駝背、沒運動習慣
        8. 家裡發生的突發狀況跟當時自己心境上的困境
        9. 自己是個守時的人
        10. 短期：點擊後端技能樹、加強技術能力；中期：在開源社群有所貢獻；長期：創業、做自己有興趣的project
* information:
    - 其實我是要面web後端RD，QA只是後來主管有興趣，前幾天臨時加的面試，結果RD當天已經沒有缺
    - 趨勢是看到cakeresume上的履歷，發email線上考邀請，以python做，約一個禮拜後約面試
    - 面試時對趨勢QA工作概況的認知：
        - by project
        - 從專案開始到最後產品上線後的使用者體驗部份全程參與
        - 有分成client端、backend等，行為模式會不同
        - 依照專案需求會碰觸到deploy
        - 該部門RD跟QA的人數比是1:1
    - 其他針對專案介紹的部份就公開紀錄
    - 環境部份：
        - 沒停車位，很難找車位
        - 電梯常常大排長龍
        - 人資很可愛...
    - 說明自己開發用過得技術時比較沒有被challange到
    - 考題很廣，以下列一些比較有印象的：
        - OS: linux指令如chmod
        - code: 給一段code考輸出
        - Web: subnet、ajax
        - 邏輯: 小明大昨天7歲，明年10歲，請問小明生日
        - testing: 針對鬧鐘app列出可做的測試、兩個client端上傳檔案到cloud要注意什麼問題
    - 遇到的人資、面試官人都還滿好的，一整天面試下來滿舒服的
* references:
    - everyting on google: `趨勢 qa 面試 ptt`
