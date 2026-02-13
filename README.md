# Claude Code notes

自分がClaude Codeを使いこなすために利用している事などをまとめる。

## 始め方

Claude Code公式サイト: https://claude.com/ja-jp/product/claude-code
公式チュートリアル: https://code.claude.com/docs/ja/overview

有料のいずれかのプラン契約後、CLI版インストール。

作業用のディレクトリを用意し、そのディレクトリでコマンドプロンプトやパワーシェルを開く。

```bash
claude
```

で起動し、あとは好きなプロンプトを入力すれば、作業を始めてくれる。

## Claude Codeのミス時のロールバックを準備する。

Claude Codeが何かしらのミスをしてしまい、少し前の状態に戻りたくなった場合に備え、ソースコード管理を行う。

ソースコード管理には、gitの利用を推奨。

git: https://git-scm.com/

GUIが必要な場合は、ほかにも使う可能性が高い機能が含まれるVisual Studio Code(VSCode)がおすすめ。

Visual Studio Code: https://code.visualstudio.com/

## Claude Codeによりプロジェクトの内容を理解させる。

Claude Codeを起動し、`/init`と指示すると、`CLAUDE.md`というファイルが作成される。

`/init`は、Claude Codeがプロジェクトを調査し、どのようなプロジェクトかを`CLAUDE.md`というファイルに書き出す。

`CLAUDE.md`は手動編集することや、claude codeに`CLAUDE.mdに、このプロジェクトでは、○○という事を追加して`などの指示で追加してくれる。

また、`/init 日本語で`と指示すれば、日本語のCLAUDE.mdを作成してくれる。
