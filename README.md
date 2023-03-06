# msamunetogetoge が主に作ったものなど

動くもの
- [NisaSimulator](https://github.com/msamunetogetoge/NisaSimulator)
  - 積立NISAでどの銘柄を買えば良いか良く分からないので、主要なインデックスの動向を見たり、購入割合を適当なアルゴリズムで計算をしてくれるアプリ。昔作ったものを育児休業中に改装した。まともに動く計算方法が一つしかないので直したいなあと思っている。bigquery + lookerとかで、インデックスのデータを見れるようにしたいなあとか思っている。
  - クライアント側はnuxtで作っていて、apiサーバーとしてpythonのFastAPIを使っている。
  - AppEngineに動いていたものをcloud build + cloud run に移行した。
  - dbはsqliteをコンテナに置いている
  
- [Nikki](https://github.com/msamunetogetoge/Nikki)
  - 日記を書くためのアプリ。ユーザー登録して日記を書いて検索できるアプリ。他のユーザーとシェアする機能を付けたいと思っていたり、セキュリティ的に良くない所があるので直したいと思っている。
  - クライアント側はnuxtで作っていて、apiサーバーとしてpythonのFastAPIを使っている。
  - gcp のcloud build + cloud run で動いている。dbはbit,io で無料のインスタンスを使っている。
  
動かないが、作ってみたもの
- [doci](https://github.com/msamunetogetoge/doci)
  - 快適にドキュメント作成をしたい、rustで何か作りたい+vueを使う練習をしたいと思って作ったアプリ。育児休業が明けたらこのアプリでドキュメント作成してやろうと思っていたが、ui/uxを上手く作れなくて開発の手が止まった。機能はgrowi というアプリを参考にした。作ったドキュメントをzipでダウンロード出来るようにしたいと思っている。
  - gcp のcloud build + cloud run で動かして開発していた。
- [autotrader](https://github.com/msamunetogetoge/AutoTrader)
  - pythonで何か作ってみようと思って殆ど初めて作った。
  - bitflyer のapiを使って、自動でbitcoinなどの取引が出来るアプリ。(ちゃんとしたアルゴリズムではないので使うのはお勧めできない。)
ブログ  
[マサムネの部屋](https://masamunetogetoge.com/)  
統計解析や機械学習を勉強していたころに書いていたブログ。
