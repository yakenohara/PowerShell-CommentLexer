`'` or `"` or `//` or `*` or `*/` を正しく判定できているかどうかを確認する  

0. `out` 配下に `QUOTE` などの出力結果ディレクトリを作っておく (`make dir.bat` バッチをたたく)

`tester.xlsm` を開いて `do` セルに TRUE を入れると、`in` フォルダ配下にある 試験用改行パターン をすべて実行する  
出力された `out` フォルダと `in` フォルダに 差分がない(Winmerge とか使って確認する) and  
`check` セルに TRUE をいれて ファイル単位のバイナリ出力差分がないことを、  
`check result` 列がすべて `~ 相違点は検出されませんでした` になるかどうかで判断する  

両方とも OK で 合格  