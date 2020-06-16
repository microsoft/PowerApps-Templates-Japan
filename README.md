---
page_type: Sample
languages: 
- Japanese
products:
- Power Apps and Power BI
description: "Power Platformを利用した軽症患者健康フォローアップシステムのサンプル"
urlFragment: "NA"
---

# Official Microsoft Sample
健康管理アプリケーションは、世界的なCOVID-19ウィルス蔓延下において、COVID-19軽症患者様の体調等の管理をする目的で作成されました。利用の用途としては、COVID-19に感染された患者様で軽症の患者様（以降軽症患者）を、一定期間別宿泊施設において健康を観察をする際に利用されるシステムで、軽症患者様用のアプリケーションと看護師様用のアプリケーション、および管理者のアプリケーションの3種類が含まれています。
アプリケーションの利用の概要としては、下記を想定しています。
軽症患者様が宿泊施設において、日々の体温や健康状況を登録をする。
看護師様は、軽症患者様の状況を把握でき、または代理で健康情報などを登録したり、コメントを入力することができる。
管理者様は、上記のアカウントなどデータの管理を行う事ができる。
上記により、軽症患者様と看護師様のコミュニケーションを物理的な接触をすることなく安全にかつ円滑にコミュニケーションをIT技術を利用して行うことができるようになります。
<!-- 
Guidelines on README format: https://review.docs.microsoft.com/help/onboard/admin/samples/concepts/readme-template?branch=master

Guidance on onboarding samples to docs.microsoft.com/samples: https://review.docs.microsoft.com/help/onboard/admin/samples/process/onboarding?branch=master

Taxonomies for products and languages: https://review.docs.microsoft.com/new-hope/information-architecture/metadata/taxonomies?branch=master

Give a short description for your sample here. What does it do and why is it important?
-->

## Contents
本レポジトリには下記のコンテンツが含まれています。

| File/folder                     　　　　　| Description                                              |
|------------------------------------------|----------------------------------------------------------|
| `FukushiFollowUp_1_0_1_1.zip`   　　　　　|Power Apps Unmanaged Solution File                        |
| `印刷用_軽症状患者レポート_提出版.pbit`   |Power BI Template File                        |
| `未提出者チェックレポート_提出版.pbit`   　|Power BI Template File                        |
| `.gitignore`                             | Define what to ignore at commit time.                    |
| `CHANGELOG.md`                           | List of changes to the sample.                           |
| `CONTRIBUTING.md`                        | Guidelines for contributing to the sample.               |
| `README.md`                              | This README file.                                        |
| `LICENSE`                                | The license for the sample.                              |

## Prerequisites

本サンプルは、Microsoft Power Apps上で動作します。
そのため、必要なライセンスもしくは評価環境のテナントを取得し評価を行っていただく必要があります。

## Setup

本サンプルでは、大きく分け2つのセットアップが必要になります。
Power Appsについては、ファイル（）をアンマネージドソリューションとして登録しています。こちらのアンマネージソリューションをソリューションのインポートでPower Appsの環境に登録をしてください。
Power BIについては、Power BIテンプレートファイル（pbit）を登録しています。こちらのデータソースを変更しご利用ください。

## Running the sample

サンプルの実行については、ソリューションファイルをインポート後、一般的なPower Apps のアプリケーションと同様に利用を行う事が可能です。
Power Apps のアプリには、ユーザーの適切なアクセス権およびPower Apps のセキュリティロールを設定する必要があります。セキュリティロールには、患者用、看護師用、管理者用の3つがあります。
Power BIレポートについては、Power BIへ発行後アクセスを行う事が可能になります。

## Key concepts
## 構成内容
本テンプレートは下記の要素にて構成されています。
Power Apps ソリューションファイル
Power Apps ソリューションファイルには次の内容が含まれています。
 - エンティティ
 - キャンバスアプリ（軽症患者様用、看護師様用）
 - モデル駆動型アプリ（システム管理者様用）
 - セキュリティロールファイル
 - その他構成ファイル
 - データ可視化用ファイル（Power BI：PBITファイル）

## 展開・利用に必要な項目
本テンプレートを展開・利用するには有償のPower AppsライセンスおよびPower BIのライセンスが必要です。詳しくは下記をご参照下さい。
https://powerapps.microsoft.com/ja-jp/pricing/
https://powerbi.microsoft.com/ja-jp/pricing/

## 必要なPower Platformの環境
本ソリューションを利用するには、Power Platform の環境（CDS：Common Data Serviceの環境）が作成されている必要があります。

## 準備されている言語
本テンプレートは日本語で準備されており、日本語にのみ対応します。

## 主な機能
主な機能は、下記のとおりです。
健康フォローアップ報告アプリ
健康フォローアップ報告アプリは、軽症患者様が日々の体温及び体調などを報告するためのアプリケーションです。
本アプリケーションの利用は、軽症患者様のスマートフォンにPower Apps アプリケーションをインストールし、配布されたアカウントにてサインインすることにより利用することができます。
利用できる主な機能は、体温の登録、パルスオキシメーター値の登録、日々の健康情報及びコメント等を登録することが可能です。

健康フォローアップ報告アプリ（看護師タブレット版）
健康フォローアップ報告アプリ（看護師タブレット版）は、看護師様が軽症患者様の日々の体調などを確認、代理入力を行うためのアプリケーションです。
本アプリケーションの利用は、タブレットもしくはWebブラウザを想定しています。配布された看護師用アカウントにてサインインすることにより利用することが可能です。
利用できる主な気のは、軽症患者様の体調の確認、代理登録、コメント入力等です。

健康フォローアップ管理アプリ
健康フォローアップ管理アプリは、管理者用のアプリケーションです。
本アプリケーションの利用は、Web ブラウザを想定しています。
利用できる主な機能は、軽症患者様の基本情報の登録、看護師様の基本情報の登録、宿泊施設などの基本情報の登録などです。

レポート
印刷用_軽症状患者レポート_提出版（印刷用_軽症状患者レポート_提出版.pbit)
ホテル滞在中の軽症状患者の体調データを患者単位で参照可能なレポートです。
印刷時にA4サイズで印刷可能なレポートサイズに設定しています。 

未提出者チェックレポート_提出版(未提出者チェックレポート_提出版.pbit)
体調データの提出状況をホテル単位で確認するためのレポートです。

## FAQ
 - Q.内容や機能をカスタマイズすることは可能ですか？
   - A.可能です。
 - Q.サポートはありますか？
    - A.いいえ、ありません。サンプルとしての提供になりますので、ご利用者様の判断にてご利用ください。
 - Q.評価版にて利用することができますか？
    - A.Power Apps及びPower BIは、双方とも30日の無償評価版があります。評価版にてご利用、機能の確認を行う事が可能です。


## Contributing
## 免責事項
本テンプレートはサンプルであり、Microsoft Power Appsにおいて、参考情報の提供等の目的で公開されています。本テンプートおよび関連サービスは、恒久的なアプリケーション使用を意図したものではありません。日本マイクロソフトはそのような目的で本テンプレートおよび関連サービスを使用するライセンスや権利を本テンプレート利用組織に付与していません。 本テンプレートおよび関連サービスは、各企業のニーズを全て含めるように設計されたものではなく、そのような用途で使用されるものではありません。実際の利用や必要な追加のカスタマイズは別途導入支援パートナーに確認・依頼してください。 本テンプレートおよび関連サービスのいかなる使用においても、利用者がすべてリスクと責任を負うものとします。また、実装した本テンプレートおよび関連マイクロソフト サービスの使用に関して、適切な警告や情報をエンドユーザーに提供することについても、利用者が責任を負うものとします。 本テンプレートは、日本国内での使用のみを目的とし、欠陥などがある可能性を含んだままの状態で提供されており、いかなる種類の保証も適用されません。

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
