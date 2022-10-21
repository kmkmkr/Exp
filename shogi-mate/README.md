# shogi-mate

詰将棋棋譜データとSeqGANから新たな詰将棋棋譜データを生成

詰将棋棋譜：https://yaneuraou.yaneu.com/2020/12/25/christmas-present/

手順

- cshogiライブラリを用いて詰将棋棋譜データ（fsen形式）->hcps形式に変換
- hcps形式を入力としseqGANで学習
- seqGANの出力（単語ID)->hcps形式に変換
- 変換したものをcshogiで読み込み盤面表示
