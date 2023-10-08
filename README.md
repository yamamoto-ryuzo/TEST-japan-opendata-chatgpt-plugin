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
 
# 用語の定義  
 https://search.ckan.jp/api　より抜粋
- xckan_original_id : 元のサイトでのデータセットID  
- xckan_title : データセットのタイトル  
- xckan_site_name : サイト名（横断検索システムで定義しています）  
- xckan_site_url : このメタデータの情報を表示するウェブサイトのURL  
- xckan_last_updated : このメタデータの最終更新日時  

# 検証していくフローの概要は下記の通り
![image](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/assets/86514652/f1801460-f19e-4336-a902-7fb7fd852c26)
