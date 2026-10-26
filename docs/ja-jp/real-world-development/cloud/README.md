---
slug: ja-jp/real-world-development/cloud
title: "GitHub Copilot クラウド エージェント"
authors:
  - geektrainer
lastUpdated: 2026-06-30
---

**[GitHub Copilot クラウド エージェント](https://docs.github.com/copilot/concepts/agents/cloud-agent/about-cloud-agent)** を使うと、GitHub Copilot がクラウドで非同期に作業できます。GitHub で作業を割り当てると、クラウド エージェントがバックグラウンドでリポジトリを調査し、変更を加え、プルリクエストを作成します。その間、ほかの作業を続けられます。

この演習では、まずクラウド エージェントが従うカスタム指示を追加し、次に GitHub issue を割り当てて実装を任せます。カスタム エージェントをレビューして使用し、エージェントの進め方を調整します。エージェント ダッシュボードからセッションの進捗を監視して指示し、最後にプルリクエストをレビューして結果を改善します。

## 演習

| 演習 | トピック | 説明 |
|----------|-------|-------------|
| [0. 前提条件][ex0] | セットアップ | リポジトリと Codespace を作成する |
| [1. カスタム指示][ex1] | コンテキスト | クラウド エージェントが従うカスタム指示を追加する |
| [2. クラウド エージェント][ex2] | 非同期エージェント | GitHub issue を GitHub Copilot クラウド エージェントに割り当てる |
| [3. カスタム エージェント][ex3] | 専門エージェント | カスタム エージェントをレビューして使用する |
| [4. エージェントの管理][ex4] | 監視 | エージェント セッションを監視して指示する |
| [5. 反復して改善][ex5] | レビュー | プルリクエストをレビューし、Copilot の作業を改善して、次の手順を選ぶ |

## 前提条件

このワークショップに参加する前に、次の準備をしてください。

- [ ] **Copilot Student、Pro、Pro+、Business、Enterprise** のいずれかの有効なプランがある GitHub アカウント
- [ ] アカウントまたは組織で GitHub Copilot クラウド エージェントが有効になっていること

> [!TIP]
> 有料プランがありませんか？在学確認済みの学生は、[GitHub Education][callout-student-plan-education] を通じて GitHub Copilot を無料で利用できます。**Copilot Student** プランには、このワークショップで使用するエージェント、MCP、コード レビュー、Copilot CLI の機能が含まれているため、すべての環境で演習を完了できます。

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> クラウド エージェントは **Copilot Student、Pro、Pro+、Business、Enterprise** で利用できます。Copilot Free では利用できません。Copilot Business または Enterprise では、管理者が組織で有効にする必要があります。

> [!NOTE]
> このワークショップでは MCP を扱いません。Copilot で MCP サーバーを使用する方法については、[CLI 環境][cli]または [VS Code 環境][vscode]を参照してください。

## はじめに

**[演習 0: 前提条件から始める →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-custom-instructions/
[ex2]: 2-cloud-agent/
[ex3]: 3-custom-agents/
[ex4]: 4-managing-agents/
[ex5]: 5-iterating/
[cli]: ../cli/
[vscode]: ../vscode/
