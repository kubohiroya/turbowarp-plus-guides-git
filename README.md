# プラとモコのGit教室

Scratch作品の変更を読み、必要なものだけ履歴に残して、仲間と共有する流れを学びます。 Hiroya Kubo が制作した、プラとモコの紙芝居1作品です。SB3に収録した6単元は目次から選べます。

- [機能・操作を学ぶ文書](docs/index.html)
- [紙芝居のSB3](docs/work/git-4.0.sb3)
- [題名・セリフ・クイズの編集元](story/lesson.ts)
- [読み進め方の検証](verification/reader-pacing.json)

文書をブラウザーで読むには、Node.js 24以上で `npm run preview` を実行し、http://127.0.0.1:8797/ を開きます。作品を試すには、SB3をTurboWarp Plus Editorで開き、実行画面を表示して緑の旗を押します。▼が点滅したらステージをクリックするかSpaceを押して進めます。

```sh
npm ci --ignore-scripts
npm run prepare:app
npm run build
```

固定した公式App 4.0.21のベースSB3とbuilderを使います。上の手順で `story/git.k4.yml`、素材SVG、`docs/work/git-4.0.sb3` と生成記録を再生成できます。

素材や出所は [NOTICE.md](NOTICE.md) を参照してください。
