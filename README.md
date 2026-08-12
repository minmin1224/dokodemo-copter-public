# どこでもコプター

ブラウザだけで3D地球儀を操縦して大空を飛び回れるフライト体験アプリです。世界の名所へワンタップで移動し、テイクオフしたらそのまま自由に飛行できます。

- インストール不要、ブラウザだけで動作します
- 通常は無料のOpenStreetMap地図でそのまま遊べます(登録不要)
- 任意でGoogle Maps Platform(Map Tiles API)のAPIキーを設定すると、実写のようなフォトリアル3D地形・建物で飛行できます
- APIキーは端末内(localStorage)にのみ保存され、外部サーバーには送信されません

## 公開URL

`index.html` がランディングページ、`app/index.html` がアプリ本体です。GitHub Pagesではリポジトリのルート(このファイル)がそのまま公開されます。

## ローカルでの動作確認

```
python -m http.server 8000
```

その後 `http://localhost:8000/` を開いてください。CesiumJSがWeb Workerを使用するため、`file://`で直接開くと正しく動作しません。
