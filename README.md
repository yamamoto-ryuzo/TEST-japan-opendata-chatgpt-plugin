# TEST-japan-opendata-chatgpt-plugin  
このページは　[japan-opendata-chatgpt-plugin](https://github.com/FooQoo/japan-opendata-chatgpt-plugin/blob/main/docs/usage.md#japan-opendata%E3%83%97%E3%83%A9%E3%82%B0%E3%82%A4%E3%83%B3%E3%81%AE%E4%BD%BF%E3%81%84%E6%96%B9)　の動作検証用のページです。  

※なぜこのプラグインが必要なのか！？  
　このプラグインを利用することで、ChatGPT(プラグインなし)・Bing・Bardと比較して、より正確にオープンデータに関する情報を検索することが可能となります。  
 
### LEVLE1 市区町村検索 
 - test1. [データカタログ横断検索システムとの比較](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/blob/main/%E3%83%87%E3%83%BC%E3%82%BF%E3%82%AB%E3%82%BF%E3%83%AD%E3%82%B0%E6%A8%AA%E6%96%AD%E6%A4%9C%E7%B4%A2%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E3%81%A8%E3%81%AE%E6%AF%94%E8%BC%83.md)  
 - test2. [検索結果に対して制御が出来るかの確認](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/blob/main/%E6%A4%9C%E7%B4%A2%E7%B5%90%E6%9E%9C%E3%81%AB%E5%AF%BE%E3%81%97%E3%81%A6%E5%88%B6%E5%BE%A1%E3%81%8C%E5%87%BA%E6%9D%A5%E3%82%8B%E3%81%8B%E3%81%AE%E7%A2%BA%E8%AA%8D.md)   
 - test3. [類義語による検索](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/blob/main/%E9%A1%9E%E7%BE%A9%E8%AA%9E%E3%81%AB%E3%82%88%E3%82%8B%E6%A4%9C%E7%B4%A2%20.md)
### LEVLE2　都道府県検索
 - [都道府県指定による市区町村横断検索](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/blob/main/%E9%83%BD%E9%81%93%E5%BA%9C%E7%9C%8C%E6%8C%87%E5%AE%9A%E3%81%AB%E3%82%88%E3%82%8B%E5%B8%82%E5%8C%BA%E7%94%BA%E6%9D%91%E6%A8%AA%E6%96%AD%E6%A4%9C%E7%B4%A2.md)

### 今後必要になるシステム  
　定期的にオープンデータのリンク切れをチェックして、修正を促すメールを送るシステム？  

# 用語の定義  
 [https://search.ckan.jp/api](https://search.ckan.jp/api)　より抜粋
- xckan_original_id : 元のサイトでのデータセットID  
- xckan_title : データセットのタイトル  
- xckan_site_name : サイト名（横断検索システムで定義しています）  
- xckan_site_url : このメタデータの情報を表示するウェブサイトのURL  
- xckan_last_updated : このメタデータの最終更新日時  

# 検証していくフローの概要は下記の通り
![image](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/assets/86514652/948ace0c-f595-4db6-964d-4f1ae3104525)

# 最新の呪文例  
### 基本形
市区町村＝「東京都」   
検索情報＝「子育て支援施設」  
抽出情報＝検索情報  
とします。  
市区町村　検索情報　に関するオープンデータをデータカタログ横断検索システムより取得して、タイトルのみに　抽出情報　 が含まれているものだけを正確に抽出し、データセットのタイトルだけを教えてください。  
ただし、市区町村　に　都道府県名が設定された場合は、「都道府県が設定されたため、まず都道府県全体を対象い検索を行った後に、市区町村ごとに検索を行います。」と表示してつぎの手順により行ってください。  
1.まず、都道府県全体を対象に検索を行ってください。  
2.都道府県の　それぞれの市区町村をわかる範囲で表示してください。  
3.それぞれの市区町村毎に　検索情報　に関するオープンデータをデータカタログ横断検索システムより取得して、返ってきたデータセットを一つ一つ確認し 、タイトルのみに 抽出情報 が含まれているものだけを正確に抽出し、データセットのタイトルだけを教えてください。  
4.次の検索は、30秒間のインターバルを設けて、自動的に続けてください。  
5.すべての検索が終了したら、市区町村およびタイトルをURL付きで一覧にしてください。  
### 類義語  
検索情報　の類似語を表示し、それぞれの類義語毎にて　その中データセットのタイトルに　抽出情報　を含むもののみを、データセットのタイトルのみ教えてください。  
