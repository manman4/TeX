## 美文書

### カッコについて

#### 大きなカッコ

\left と \right で囲むと、角のようになる。

https://tex.stackexchange.com/questions/173717/is-it-ever-bad-to-use-left-and-right/173771#173771

\biggl と \biggr で囲むと、角が丸くなる。

SumやProdを囲む場合は、\biggl との間が狭いので、`\,` を入れると見栄えが良くなる。

#### 大きなカッコのk乗

そのままだとk乗部分が浮いた感じになるので、`^{\!k}` にすると見栄えが良くなる。



## 文法

### ページ


```
\documentclass{book}
\usepackage{fancyhdr}
\pagestyle{fancy} % 初期設定（例えば、ヘッダーとフッターを表示）

\fancyhf{} % 初期状態ではヘッダーとフッターをクリア
\fancyhead[LE,RO]{\leftmark} % 章名を表示
\fancyfoot[LE]{\thepage} % 左ページ（偶数）の左端にページ番号
\fancyfoot[RO]{\thepage} % 右ページ（奇数）の右端にページ番号

\begin{document}

% 何らかの内容

% ページスタイルをemptyに設定（ヘッダー・フッターなし）
\pagestyle{empty}
\newpage % 新しいページを開始

% 次のページから元の設定に戻す
\pagestyle{fancy}
\newpage % 新しいページを開始

% 以下、元の設定が適用される

\end{document}

```


説明：
最初のページでは、\pagestyle{fancy} を設定して、ヘッダーやフッターを表示します。
その後、\pagestyle{empty} を使用して次のページでヘッダーとフッターを非表示にします。
新しいページで再び \pagestyle{fancy} を使用することで、元のページスタイルを適用します。

