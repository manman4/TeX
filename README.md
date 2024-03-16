# TeX

## install

### Mac

(参考)　https://zenn.dev/umi_mori/books/72d30926afbc24/viewer/473920


1.mactexのインストール

```sh
brew install mactex --cask
```

2.Terminalの再起動

3.TeXの設定

```sh
sudo tlmgr update --self --all
sudo tlmgr paper a4
```

4.アプリケーションインストールの確認


## 実行

1.texファイルの作成

2.dviファイルの作成

```sh
platex xxx.tex
```

3.pdfファイルの作成

```sh
dvipdfmx xxx
```


