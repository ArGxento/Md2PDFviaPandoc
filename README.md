---
title: Md2PDFviaPandoc
author: ArGxento
---

# Md2PDFviaPandoc

私が使っている、MarkdownからpLaTeXとPandocによって
PDFを生成するためのテンプレート一式です。

# 使い方

 1. [Pandoc](http://johnmacfarlane.net/pandoc/)と
 [OMake](http://omake.metaprl.org/index.html), pLaTeX
 を導入してください
 2. OMakefile, OMakeroot, template.tex, report.md
 の4つを適当なディレクトリにコピーしてください
 3. report.mdを適当に編集します
 4. `omake -P`を叩くと、ファイルに変更があるたびに
 コンパイルし直され、リアルタイムで確認できます
 5. ラベルの参照解消するために、完成後に`omake -U`を
 叩いた方がよさそうです

# 定義済みマクロについて
ドキュメント側からテンプレートをある程度カスタマイズ
できるように、いくつかのPandocマクロを定義してあります。
また、Markdownで書き表せないいくつかのLaTeX機能について、
TeXのマクロを定義してあります。詳細はtemplate.texを
参照してください。

# その他

TeXLive2013に標準でついてくるパッケージのみ使用する
ようにしましたが、比較的無茶苦茶なハックをかけてある
点が多いので、エラーが出るなどしたらtemplate.texを
読んでみてください。
