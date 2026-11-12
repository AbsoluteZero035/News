<h1 align="center">速報ラジオ</h1>

<p align="center"><b>キャラクターが毎朝ニュースを読む「放送局」です。</b></p>

<p align="center">AI・IT・プログラミングの、きのうの気になるニュースを、毎朝お届けします。</p>

- **配信は、台本と音声を置いて push するだけ**。サーバーはいりません
- 動画ではなく **HTML の番組**です。再生位置に合わせて、スライド・字幕・キャラ・リンクカードが動きます
- **ニュースの画像は、記事のサイトがサムネイル用に公開している画像（OGP）を参照表示します**。画像を保存したり配り直したりしません
- 番組の中身は文字の台本（JSON）です。音声はそれを読み上げたもので、公開するのは直近 30 日分だけです

## しくみ

この局は [monoradio102/myradio](https://github.com/monoradio102/myradio)（MIT License）をテンプレートとして使っています。台本と声の作り方は `AGENTS.md`、JSON の形は `docs/formats.md` にあります。

- 局の情報：`station.json`
- 台本：`episodes/<日付>-ja.json`、一覧は `episodes.json`
- 声：`audio/<日付>-ja.mp3`（この局は main ブランチからそのまま配信します。古い音声は 30 日を目安に消します）
- キャスター：`character/`（宙夢が指定した AI 生成のキャラクター画像をもとに作成）

## クレジット

- 声：音声合成（Muse / TTS）
- キャラクター：宙夢が指定した AI 生成画像
- プレーヤー：monoradio102/myradio（MIT License）
