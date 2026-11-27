# Gitの手元練習

教材を見終わった後、普段の作品とは別の空のフォルダーで試すための操作例です。ここに書いたコマンドを教材が自動実行することはありません。リモートの設定やpushは含みません。Gitをインストールし、コミットで使う名前・メールを自分の方針に合わせて設定しておきます。

1. 空の練習フォルダーへ移動し、`git init -b main` でリポジトリを作る。
2. テキストエディタで `lesson.txt` を作り、`spacing=60` と保存する。
3. `git status` で未追跡のファイルを確認する。
4. `git add lesson.txt`、`git diff --staged` で次に記録する内容を確認する。
5. `git commit -m "星の間隔の初期値を記録"` で最初の記録を作る。
6. `git switch -c experiment` で練習用の枝を作る。
7. ファイルを `spacing=70` に変更して保存し、`git diff` で前後を比べる。
8. `git add lesson.txt`、`git diff --staged`、`git commit -m "星が重ならないよう間隔を広げる"` と進める。
9. `git log --oneline --graph --all` で履歴と枝の指す先を見る。
10. 未記録の変更がないことを確認し、`git switch main`、`git merge experiment` と進める。この例ではmain側に新しい記録がないため、通常はfast-forwardになる。
11. `git status` とファイルの内容を確認する。作品なら、統合後の動作確認も行う。

この例はGitの三つの領域と、単純な枝の統合を確かめるものです。Plusの作品フォルダーでの保存形式や素材の追跡方針は、Editorの対応版とプロジェクト方針に合わせます。SB3単体のバイナリ差分を、ブロックの読みやすい行差分と同じものだと思わないようにします。
