<picture>
  <source media="(prefers-color-scheme: dark)"
          srcset="https://raw.githubusercontent.com/bidaide/.github/main/profile/assets/logo-dark.svg">
  <img src="https://raw.githubusercontent.com/bidaide/.github/main/profile/assets/logo-light.svg"
       alt="Bidaide" width="88">
</picture>

# .github

Bidaide 組織全体で共有する GitHub の設定・テンプレート類を管理するリポジトリです。

`.github` という特殊なリポジトリ名のため、Organization 内の各リポジトリに専用の Issue/PR テンプレートが無い場合、ここに置いたテンプレートがデフォルトとして自動的に適用されます。

## 含まれるもの

- `.github/ISSUE_TEMPLATE/` — Issue テンプレート（feature request / bug report / question / chore）
- `.github/PULL_REQUEST_TEMPLATE.md` — Pull Request テンプレート
- `.gitmessage` — コミットメッセージテンプレート（Conventional Commits + 絵文字）
- `.gitignore` — 共通の除外設定
- `profile/README.md` — Organization トップページに表示されるプロフィール

## コミットメッセージテンプレートの使い方

`.gitmessage` は Issue/PR テンプレートと異なり自動適用されないため、使う場合は各自のローカル環境で設定してください。

すべてのリポジトリで使う場合（グローバル設定）:

```sh
git config --global commit.template path/to/.gitmessage
```

特定のリポジトリだけで使う場合:

```sh
git config commit.template path/to/.gitmessage
```

規約の詳細は `.gitmessage` 内のコメントを参照してください。
