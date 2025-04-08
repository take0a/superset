---
hide_title: true
sidebar_position: 1
---
<!--
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# Superset

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/license/apache-2-0)
[![Latest Release on Github](https://img.shields.io/github/v/release/apache/superset?sort=semver)](https://github.com/apache/superset/releases/latest)
[![Build Status](https://github.com/apache/superset/actions/workflows/superset-python-unittest.yml/badge.svg)](https://github.com/apache/superset/actions)
[![PyPI version](https://badge.fury.io/py/apache_superset.svg)](https://badge.fury.io/py/apache_superset)
[![Coverage Status](https://codecov.io/github/apache/superset/coverage.svg?branch=master)](https://codecov.io/github/apache/superset)
[![PyPI](https://img.shields.io/pypi/pyversions/apache_superset.svg?maxAge=2592000)](https://pypi.python.org/pypi/apache_superset)
[![Get on Slack](https://img.shields.io/badge/slack-join-orange.svg)](http://bit.ly/join-superset-slack)
[![Documentation](https://img.shields.io/badge/docs-apache.org-blue.svg)](https://superset.apache.org)

<picture width="500">
  <source
    width="600"
    media="(prefers-color-scheme: dark)"
    src="https://superset.apache.org/img/superset-logo-horiz-dark.svg"
    alt="Superset logo (dark)"
  />
  <img
    width="600"
    src="https://superset.apache.org/img/superset-logo-horiz-apache.svg"
    alt="Superset logo (light)"
  />
</picture>

最新のエンタープライズ対応ビジネス インテリジェンス Web アプリケーション。

[**Superset を選ぶ理由**](#why-superset) |
[**サポートされているデータベース**](#supported-databases) |
[**インストールと構成**](#installation-and-configuration) |
[**リリース ノート**](https://github.com/apache/superset/blob/master/RELEASING/README.md#release-notes-for-recent-releases) |
[**参加する**](#get-involved) |
[**貢献者ガイド**](#contributor-guide) |
[**リソース**](#resources) |
[**Superset を使用している組織**](https://github.com/apache/superset/blob/master/RESOURCES/INTHEWILD.md)

## Superset を選ぶ理由 {#why-superset}

Superset は、最新のデータ探索およびデータ視覚化プラットフォームです。Superset は、多くのチームの独自のビジネス インテリジェンス ツールを置き換えたり、強化したりできます。Superset は、さまざまなデータ ソースと適切に統合されます。

Superset は以下を提供します:

- グラフをすばやく作成するための **コード不要のインターフェース**
- 高度なクエリを実行するための強力な Web ベースの **SQL エディター**
- カスタム ディメンションとメトリックをすばやく定義するための **軽量のセマンティック レイヤー**
- **ほぼすべての SQL** データベースまたはデータ エンジンをすぐにサポート
- シンプルな棒グラフから地理空間の視覚化まで、データを展示するための幅広い **美しい視覚化**
- データベースの負荷を軽減する軽量で構成可能な **キャッシュ レイヤー**
- 高度に拡張可能な **セキュリティ ロールと認証** オプション
- プログラムによるカスタマイズのための **API**
- 拡張性を考慮してゼロから設計された **クラウド ネイティブ アーキテクチャ**

## スクリーンショットとGIF画像

**Video Overview**

<!-- File hosted here https://github.com/apache/superset-site/raw/lfs/superset-video-4k.mp4 -->

[superset-video-1080p.webm](https://github.com/user-attachments/assets/b37388f7-a971-409c-96a7-90c4e31322e6)

<br/>

**Large Gallery of Visualizations**

<kbd><img title="Gallery" src="https://superset.apache.org/img/screenshots/gallery.jpg"/></kbd><br/>

**Craft Beautiful, Dynamic Dashboards**

<kbd><img title="View Dashboards" src="https://superset.apache.org/img/screenshots/slack_dash.jpg"/></kbd><br/>

**No-Code Chart Builder**

<kbd><img title="Slice & dice your data" src="https://superset.apache.org/img/screenshots/explore.jpg"/></kbd><br/>

**Powerful SQL Editor**

<kbd><img title="SQL Lab" src="https://superset.apache.org/img/screenshots/sql_lab.jpg"/></kbd><br/>

## サポートされているデータベース {#supported-databases}

Superset は、Python DB-API ドライバーと SQLAlchemy 方言を備えた、SQL 対応のデータストアまたはデータ エンジン (Presto、Trino、Athena など) からデータをクエリできます。

サポートされている主要なデータベース ソリューションの一部を以下に示します:

<p align="center">
  <img src="https://superset.apache.org/img/databases/redshift.png" alt="redshift" border="0" width="200"/>
  <img src="https://superset.apache.org/img/databases/google-biquery.png" alt="google-biquery" border="0" width="200"/>
  <img src="https://superset.apache.org/img/databases/snowflake.png" alt="snowflake" border="0" width="200"/>
  <img src="https://superset.apache.org/img/databases/trino.png" alt="trino" border="0" width="150" />
  <img src="https://superset.apache.org/img/databases/presto.png" alt="presto" border="0" width="200"/>
  <img src="https://superset.apache.org/img/databases/databricks.png" alt="databricks" border="0" width="160" />
  <img src="https://superset.apache.org/img/databases/druid.png" alt="druid" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/firebolt.png" alt="firebolt" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/timescale.png" alt="timescale" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/rockset.png" alt="rockset" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/postgresql.png" alt="postgresql" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/mysql.png" alt="mysql" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/mssql-server.png" alt="mssql-server" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/ibm-db2.svg" alt="db2" border="0" width="220" />
  <img src="https://superset.apache.org/img/databases/sqlite.png" alt="sqlite" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/sybase.png" alt="sybase" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/mariadb.png" alt="mariadb" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/vertica.png" alt="vertica" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/oracle.png" alt="oracle" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/firebird.png" alt="firebird" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/greenplum.png" alt="greenplum" border="0" width="200"  />
  <img src="https://superset.apache.org/img/databases/clickhouse.png" alt="clickhouse" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/exasol.png" alt="exasol" border="0" width="160" />
  <img src="https://superset.apache.org/img/databases/monet-db.png" alt="monet-db" border="0" width="200"  />
  <img src="https://superset.apache.org/img/databases/apache-kylin.png" alt="apache-kylin" border="0" width="80"/>
  <img src="https://superset.apache.org/img/databases/hologres.png" alt="hologres" border="0" width="80"/>
  <img src="https://superset.apache.org/img/databases/netezza.png" alt="netezza" border="0" width="80"/>
  <img src="https://superset.apache.org/img/databases/pinot.png" alt="pinot" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/teradata.png" alt="teradata" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/yugabyte.png" alt="yugabyte" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/databend.png" alt="databend" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/starrocks.png" alt="starrocks" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/doris.png" alt="doris" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/oceanbase.svg" alt="oceanbase" border="0" width="220" />
  <img src="https://superset.apache.org/img/databases/sap-hana.png" alt="oceanbase" border="0" width="220" />
  <img src="https://superset.apache.org/img/databases/denodo.png" alt="denodo" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/ydb.svg" alt="ydb" border="0" width="200" />
  <img src="https://superset.apache.org/img/databases/tdengine.png" alt="TDengine" border="0" width="200" />
</p>

**サポートされているデータベースのより包括的なリスト** と構成手順については、[こちら](https://superset.apache.org/docs/configuration/databases) をご覧ください。

データストアまたはデータ エンジンのサポートを追加したいですか? 技術的な要件については、[こちら](https://superset.apache.org/docs/frequently-asked-questions#does-superset-work-with-insert-database-engine-here) をご覧ください。

## インストールと構成 {#installation-and-configuration}

Superset の [クイックスタート](https://superset.apache.org/docs/quickstart/) ガイドを試すか、[本番環境への展開のオプション](https://superset.apache.org/docs/installation/architecture/) について学んでください。

## 参加する {#get-involved}

- [StackOverflow](https://stackoverflow.com/questions/tagged/apache-superset) で **apache-superset** タグを使用して質問したり回答したりしてください
- [コミュニティの Slack に参加してください](http://bit.ly/join-superset-slack)
また、[Slack コミュニティ ガイドライン](https://github.com/apache/superset/blob/master/CODE_OF_CONDUCT.md#slack-community-guidelines) をお読みください
- [dev@superset.apache.org メーリング リストに参加してください](https://lists.apache.org/list.html?dev@superset.apache.org)。参加するには、[dev-subscribe@superset.apache.org](mailto:dev-subscribe@superset.apache.org) にメールを送信するだけです。
- Superset がサポートする多数のデータベース ドライバーに関連する GitHub の問題のトラブルシューティングに協力したい場合は、[Superset データベース ファミリアビリティ ロロデックス](https://docs.google.com/spreadsheets/d/1U1qxiLvOX0kBTUGME1AHHi6Ywel6ECF8xk_Qy-V9R8c/edit#gid=0) に自分の名前とアクセスできるデータベースを追加することを検討してください。
- Superset のタウン ホールと [運用モデル](https://preset.io/blog/the-superset-operational-model-wants-you/) の定期ミーティングに参加してください。ミーティング情報は、[Superset コミュニティ カレンダー](https://superset.apache.org/community) で確認できます。

## 貢献者ガイド {#contributor-guide}

貢献に興味がありますか? [CONTRIBUTING.md](https://github.com/apache/superset/blob/master/CONTRIBUTING.md) をチェックして、貢献に関するリソースと開発環境の設定方法に関する詳細なガイドを見つけてください。

## リソース {#resources}

- [Superset "In the Wild"](https://github.com/apache/superset/blob/master/RESOURCES/INTHEWILD.md) - PR を開いて、組織をリストに追加してください。
- [機能フラグ](https://github.com/apache/superset/blob/master/RESOURCES/FEATURE_FLAGS.md) - Superset の機能フラグのステータス。
- [標準ロール](https://github.com/apache/superset/blob/master/RESOURCES/STANDARD_ROLES.md) - RBAC 権限がロールにマップされる方法。
- [Superset Wiki](https://github.com/apache/superset/wiki) - ベスト プラクティス、コミュニティ コンテンツ、その他の情報など、多数の追加コミュニティ リソース。
- [Superset SIP](https://github.com/orgs/apache/projects/170) - Superset の SIP (Superset 改善提案) のコンセンサスと実装ステータスの両方のステータス。

スーパーセットの視点を理解する

- [データセット中心の視覚化の事例](https://preset.io/blog/dataset-centric-visualization/)
- [スーパーセット セマンティック レイヤーの理解](https://preset.io/blog/understanding-superset-semantic-layer/)

- Superset を使い始める
  - [Docker Compose を使用して 2 分で Superset を作成する](https://superset.apache.org/docs/installation/docker-compose#installing-superset-locally-using-docker-compose)
  - [データベース ドライバーのインストール](https://superset.apache.org/docs/configuration/databases#installing-database-drivers)
  - [新しいデータベース コネクタの構築](https://preset.io/blog/building-database-connector/)
  - [最初のダッシュボードの作成](https://superset.apache.org/docs/using-superset/creating-your-first-dashboard/)
  - [Apache Superset へのコード提供に関する包括的なチュートリアル](https://preset.io/blog/tutorial-contributing-code-to-apache-superset/)
- [Preset による Superset の習得に役立つリソース](https://preset.io/resources/)

- Superset のデプロイ

  - [公式 Docker イメージ](https://hub.docker.com/r/apache/superset)
  - [Helm Chart](https://github.com/apache/superset/tree/master/helm/superset)

- 過去の[Supersetコミュニティイベント](https://preset.io/events)の録画

  - [混合時系列チャート](https://preset.io/events/mixed-time-series-visualization-in-superset-workshop/)
  - [Bing チームが社内セルフサービス データ & アナリティクス プラットフォーム用に Superset をカスタマイズした方法](https://preset.io/events/how-the-bing-team-heavily-customized-superset-for-their-internal-data/)
  - [ライブ デモ: Trino を使用して MongoDB と Pinot のデータを視覚化する](https://preset.io/events/2021-04-13-visualizing-mongodb-and-pinot-data-using-trino/)
  - [Superset API の概要](https://preset.io/events/introduction-to-the-superset-api/)
  - [Superset 用のデータベース コネクタの構築](https://preset.io/events/2021-02-16-building-a-database-connector-for-superset/)

- 視覚化

  - [Viz プラグインの作成](https://superset.apache.org/docs/contributing/creating-viz-plugins/)
  - [カスタム Viz プラグインの管理と展開](https://medium.com/nmc-techblog/apache-superset-manage-custom-viz-plugins-in-production-9fde1a708e55)
  - [Apache Superset が Apache ECharts に賭ける理由](https://preset.io/blog/2021-4-1-why-echarts/)

- [スーパーセット API](https://superset.apache.org/docs/rest-api)

## リポジトリアクティビティ

<a href="https://next.ossinsight.io/widgets/official/compose-last-28-days-stats?repo_id=39464018" target="_blank" align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://next.ossinsight.io/widgets/official/compose-last-28-days-stats/thumbnail.png?repo_id=39464018&image_size=auto&color_scheme=dark" width="655" height="auto" />
    <img alt="Performance Stats of apache/superset - Last 28 days" src="https://next.ossinsight.io/widgets/official/compose-last-28-days-stats/thumbnail.png?repo_id=39464018&image_size=auto&color_scheme=light" width="655" height="auto" />
  </picture>
</a>

<!-- Made with [OSS Insight](https://ossinsight.io/) -->

<!-- telemetry/analytics pixel: -->
<img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=bc1c90cd-bc04-4e11-8c7b-289fb2839492" />
