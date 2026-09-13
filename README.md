# Homebrew tap for kilde

[kilde](https://github.com/takezou621/kilde) の Homebrew tap です。

## インストール

tap を追加してからインストールします。

```sh
brew tap takezou621/kilde
brew trust --formula takezou621/kilde/kilde   # 新しい Homebrew のセキュリティモデルで必要 (初回 1 回)
brew install kilde
```

tap の追加とインストールを 1 コマンドで行うこともできます。

```sh
brew install takezou621/kilde/kilde
```

## HEAD 版

最新の `main` ブランチをソースからビルドする場合は `--HEAD` を指定します。
Xcode 26 SDK 以降が必要です (macOS 26 の `captureHDRRecordingPreservedSDRHDR10` を参照するため、旧 SDK ではビルドできません。実行は macOS 14+ に対応します)。

```sh
brew install --HEAD takezou621/kilde/kilde
```

## BlackHole

BlackHole は必須ではありません。録音しながら同じ音を聞くモニター経路を使う場合だけ、
次のコマンドで追加してください。

```sh
brew install --cask blackhole-2ch
```

インストール後、初回は `kilde doctor` で画面収録・マイクの権限を確認してください。
