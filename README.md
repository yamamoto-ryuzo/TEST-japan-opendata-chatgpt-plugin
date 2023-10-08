# TEST-japan-opendata-chatgpt-plugin  
このページは　[japan-opendata-chatgpt-plugin](https://github.com/FooQoo/japan-opendata-chatgpt-plugin/blob/main/docs/usage.md#japan-opendata%E3%83%97%E3%83%A9%E3%82%B0%E3%82%A4%E3%83%B3%E3%81%AE%E4%BD%BF%E3%81%84%E6%96%B9)　の動作検証用のページです。  
- test1. [データカタログ横断検索システムとの比較](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/blob/main/%E3%83%87%E3%83%BC%E3%82%BF%E3%82%AB%E3%82%BF%E3%83%AD%E3%82%B0%E6%A8%AA%E6%96%AD%E6%A4%9C%E7%B4%A2%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E3%81%A8%E3%81%AE%E6%AF%94%E8%BC%83.md)  
- test2. [検索結果に対して制御が出来るかの確認](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/blob/main/%E6%A4%9C%E7%B4%A2%E7%B5%90%E6%9E%9C%E3%81%AB%E5%AF%BE%E3%81%97%E3%81%A6%E5%88%B6%E5%BE%A1%E3%81%8C%E5%87%BA%E6%9D%A5%E3%82%8B%E3%81%8B%E3%81%AE%E7%A2%BA%E8%AA%8D.md)   

# 用語の定義  
 https://search.ckan.jp/api　より抜粋
- xckan_original_id : 元のサイトでのデータセットID  
- xckan_title : データセットのタイトル  
- xckan_site_name : サイト名（横断検索システムで定義しています）  
- xckan_site_url : このメタデータの情報を表示するウェブサイトのURL  
- xckan_last_updated : このメタデータの最終更新日時  

### 検証していくフローの概要は下記の通り
　![image](https://github.com/yamamoto-ryuzo/TEST-japan-opendata-chatgpt-plugin/assets/86514652/d5db3aab-a736-4d75-a00b-8561ff5dd26d)
  
