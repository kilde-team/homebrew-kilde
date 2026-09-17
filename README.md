# Homebrew tap for kilde

[kilde](https://github.com/kilde-team/kilde) の Homebrew tap です。

## インストール

tap を追加してからインストールします。

```sh
brew tap kilde-team/kilde
brew trust --formula kilde-team/kilde/kilde   # 新しい Homebrew のセキュリティモデルで必要 (初回 1 回)
brew install kilde
```

tap の追加とインストールを 1 コマンドで行うこともできます。

```sh
brew install kilde-team/kilde/kilde
```

## BlackHole

BlackHole は必須ではありません。録音しながら同じ音を聞くモニター経路を使う場合だけ、
次のコマンドで追加してください。

```sh
brew install --cask blackhole-2ch
```

インストール後、初回は `kilde doctor` で画面収録・マイクの権限を確認してください。
