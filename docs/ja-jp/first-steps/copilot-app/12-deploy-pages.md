---
title: "レッスン 12 - GitHub Pages でサイトを公開する"
description: "GitHub Copilot アプリを使って Pages ワークフローを設定し、そのプルリクエストをレビューして、公開された Space Quiz を確認します。"
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Space Quiz を公開して、誰でもアクセスできるようにしましょう。Copilot はワークフローの準備とデプロイを支援しますが、変更をレビューし、サイトが公開されたことを確認するのは自分の役割です。

このレッスンでは、次のことを行います。

- Copilot に GitHub Pages のデプロイ設定を依頼します。
- マージする前にワークフローとプルリクエストをレビューします。
- デプロイの進行状況を確認し、公開されたサイトを検証します。

## シナリオ

Space Quiz はすでに GitHub リポジトリにありますが、誰でも簡単に試せるようにする必要があります。単一ファイルのサイトを GitHub Pages で公開すると、サーバーやランタイム依存関係を追加せずに、公開 URL からアクセスできるようになります。

## Copilot にサイトの公開を依頼する

`space-quiz` 用の Copilot アプリ セッションで、次のプロンプトを送信します。

```plaintext
Enable GitHub Pages for this repository. Create a GitHub Actions workflow that builds the website if needed and deploys it to GitHub Pages. Add a README describing the app and how to run it locally if one does not already exist. Create a pull request with these changes and merge it after required checks pass. Monitor the deployment until it succeeds, then report the final URL of the live website. If you lack permission to enable Pages or merge, tell me exactly what I need to approve or do; do not report success until the site is live.
```

![3 段階の図: マージ済みの space-quiz プルリクエスト、Build website・Upload artifact・Deploy to Pages の各手順が成功した GitHub Actions の Deploy website 実行、yourname.github.io/space-quiz/ で公開された Space Quiz。](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> このプロンプトは、エージェントにプルリクエストの作成とマージ、およびリポジトリの Pages 設定の変更を依頼します。続行する前に、diff、デプロイ権限、GitHub に表示される承認要求を確認してください。

## ワークフローをレビューしてデプロイを確認する

1. リポジトリに README がない場合に限り、README が追加されていることを確認します。
2. ワークフローのビルド手順とデプロイ手順を含め、プルリクエストの変更をレビューします。
3. プルリクエストの必須チェックに合格してからマージします。
4. GitHub Actions のデプロイ実行を、成功するまで確認します。
5. 報告された URL を開き、Space Quiz が読み込まれることを確認します。

エージェントが Pages の有効化やプルリクエストのマージを実行できない場合は、提示された具体的な手順に従ってください。デプロイが成功し、公開サイトが読み込まれるまでは、完了とみなさないでください。

## まとめと次のステップ

Space Quiz が公開され、エージェントの報告だけに頼らず、デプロイを確認できました。続けて[レッスン 13: 振り返りと次のステップ][next-lesson]に進みます。

[next-lesson]: ../13-review/
