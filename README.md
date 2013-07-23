簡介
===


「漢字標準格式」是基於樣式「重設」及「標準化」二個概念寫成的CSS3排版框架。由於現今的瀏覽器預設樣式皆以西文顯示為主，未能周詳地考慮到其與漢字排版間的差異，嚴重影響美觀度，造成網頁設計師的誤用，更使得內容編者無從依照語意正確使用字級元素。

「樣式標準化」的想法源自網上諸多CSS reset及「normalize.css」專案，經漢字標準格式的沿用、加入特定語種的支援，並將漢字文化圈中常見的印刷品排印格式套用在各種HTML5元素中，從而提供標準合理而美觀的文章閱讀環境，迎合網頁讀者的閱讀習慣及設計師和編者的需求。

漢字標準格式目前可完整支援繁體中文、簡體中文及日文等三種漢字形式的網頁。



啓用設置步驟
---

1. 在欲套用「漢字標準格式」CSS框架的網頁中、所有樣式宣告*之前*導入下列外連樣式表：

    	<link rel="stylesheet" media="all" href="./css/han.css">

2. 同上，再加入以下JavaScript語法：

    	<script src="http://ajax.googleapis.com/ajax/libs/jquery/2.0.2/jquery.min.js"></script>
    	<script src="./han.min.js"></script>

3. 留意`<html>`標籤上是否設置了正確的語言屬性`lang`。此框架多數功能僅支援中文`zh-*`及日語`ja`。

4. 在瀏覽器中開啓已套用本框架的網頁測試是否正確運作。


***


### 啓用注音符號支援

由於使用頻率較低，「漢字標準格式」將`<ruby>`中的「直式注音符號支援」同主程式分離，需另行啓用方可正確顯示此功能之效果。

1. 開啓`han.zhuyin.css`，將「188、189行」的`../fonts/zhuyin.eot`及`../fonts/zhuyin.ttf`重新定向至正確的檔案路徑。

    **請注意：**此處使用的注音符號字體係由中華民國教育部所研發的「[教育部標準楷書][kai]」，並採**[創用CC「姓名標示–禁止改作–3.0–台灣版」][cc]授權**。若你有著作權的疑慮，請直接刪除上述提及之二行代碼及檔案，「漢字標準格式」將自動fallback至使用者作業系統的漢字手寫字體。

2. 開啓`han.css`，將「65行」的代碼由註解範圍*更改*為一般代碼格式。

3. 在瀏覽器中開啓內含`<ruby class="zhuyin"> … </ruby>`元素的網頁進行測試。


[kai]: http://www.edu.tw/treasure/filedown.aspx?Node=1123&Index=2&WID=c5ad5187-55ef-4811-8219-e946fe04f725
[cc]: http://creativecommons.org/licenses/by-nd/3.0/tw/


***


「漢字標準格式」版本：v2.0.0  
最後修改於：2013年7月23日 18:24（GMT+8）





