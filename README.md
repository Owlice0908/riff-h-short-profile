# riff-h-short-profile

Riff-H-Short 配布パッケージ向けの **公開 profile.yaml** リポジトリ。

## 用途

このリポジトリの `profile.yaml` は、Riff-H-Short の各配布インストールから
`/profile/update` エンドポイント経由で自動取得されます。

更新フロー:
1. `profile.yaml` を編集
2. `version:` 行を上げる (例: `1.0` → `1.1`)
3. `git commit && git push`
4. 配布先で「プロファイル更新」ボタンを押すと反映

## URL

各配布パッケージの `config.yaml` の `profile_update_url` には以下を設定:

```
https://raw.githubusercontent.com/Owlice0908/riff-h-short-profile/main/profile.yaml
```
