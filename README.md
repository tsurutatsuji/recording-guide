# recording-guide

一人称視点クリップの撮り方1ページ。撮影者にリンクで配る。

公開URL: https://tsurutatsuji.github.io/recording-guide/

## 人ごとにURLを差し替える

`index.html` は3つのURLパラメータを読む。1ファイルを人数分に使い回せる。

| パラメータ | 効果 |
|---|---|
| `name` | 見出しに名前が入る |
| `due` | 納期の欄を差し替える |
| `tasks` | 割り当て作業を `|` 区切りで並べる。無ければ「チャットの一覧を見て」と表示 |

例:
```
https://tsurutatsuji.github.io/recording-guide/?name=Zamzam&due=Wednesday%2C+5+August+2026&tasks=Wiping+a+table%7CFolding+laundry
```

## 更新のしかた

`index.html` を直して push すれば、配ったリンク全部が即座に最新になる。

```
git add -A && git commit -m "…" && git push
```

## 将来

規格に検査票や価格が入る段階になったら、ソースを非公開にできる Cloudflare Pages へ移す（HTMLを移すだけ）。
