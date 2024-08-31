# Power Apps YAML Source Code: File Uploader Component
**(ja-jp) Power Appsのコンポーネント: ファイルアップローダー**

<a href="https://x.com/DemodoriGatsuo"><img src="https://img.shields.io/twitter/follow/DemodoriGatsuo"/></a>

![Power Apps](https://img.shields.io/badge/-Power%20Apps-742774?style=flat-square&logo=powerapps&logoColor=white)
![SharePoint](https://img.shields.io/badge/-SharePoint-038387?style=flat-square&logo=microsoft-sharepoint&logoColor=white)

## Overview

This component enables direct file uploads to a folder in a SharePoint document library from Power Apps. It utilizes the Office 365 Groups connector to achieve file uploads.

Power AppsからSharePointのドキュメントライブラリのフォルダに直接ファイルアップロードを実現するコンポーネントです。
Office 365 Groupsコネクタを用いてファイルアップロードを実現しています。

[Qiitaによる技術記事](https://qiita.com/DEmodoriGatsuO/items/2b9c25cf5dcd17b4958d)

Visit https://qiita.com/DEmodoriGatsuO/items/2b9c25cf5dcd17b4958d

Since the source code is written in YAML, you can use it in Power Apps simply by copying and pasting, even if you don't use it as a component. Please utilize it according to your environment.

The component requires four input values.

`YAML ソースコード`で記載しているため、コンポーネントとして利用しなくても、コピー&ペーストで`Power Apps`で利用することができます。
環境に合わせてご活用ください。

コンポーネントでは4つの入力値を求めています。

## Custom Properties
**Input**

|Properties|Description|
|---|---|
|`site_id`|SharePoint SiteId|
|`drive_id`|SharePoint Drive ID|
|`folder_name`|Folder Name|
|`static_icon_table`|Table defining file types and extensions|

**Output**

|Properties|Description|
|---|---|
|`response`|Custom property for responses (Output)


### Reference
- [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer) - https://developer.microsoft.com/en-us/graph/graph-explorer
- [Power Apps DIRECTLY upload files to SharePoint Document Library | GRAPH API](https://youtu.be/n3mhe88BI34?si=xtlIrg0u84fLQP-Q) - https://youtu.be/n3mhe88BI34?si=xtlIrg0u84fLQP-Q
- [Error、IfError、IsError、IsBlankOrError 関数](https://learn.microsoft.com/ja-jp/power-platform/power-fx/reference/function-iferror) - https://learn.microsoft.com/ja-jp/power-platform/power-fx/reference/function-iferror
- [Office 365 Groups](https://learn.microsoft.com/ja-jp/connectors/office365groups/) - https://learn.microsoft.com/ja-jp/connectors/office365groups/
- [YouTube](https://www.youtube.com/embed/n3mhe88BI34?si=xtlIrg0u84fLQP-Q)

## Usage

### Setting Up

1. **Define Properties**: Set the `site_id`, `drive_id`, `folder_name`, and `static_icon_table` properties with appropriate values.
2. **Configure Attachments**: Ensure the `OnAddFile` property in the `Attachments` control is correctly set up to handle file uploads to SharePoint.
3. **Customize Layout**: Adjust the layout and styling properties as needed to fit the design requirements.

1. **プロパティの定義**： `site_id`、`drive_id`、`folder_name`、`static_icon_table`をご自身の環境に合わせて設定してください。
2. **添付ファイル コントロール**： `添付ファイル コントロール`の`OnAddFile` プロパティが `SharePoint`へのファイルアップロードを処理するために正しく設定されていることを確認してください。
3. **レイアウトのカスタマイズ**： デザイン要件に合うように、必要に応じてレイアウトとスタイリングのプロパティを調整します。

### Customization

- **Add New File Types**: Update the `static_icon_table` property to include additional file types and their corresponding extensions.
- **Modify Layout**: Adjust the properties of the GroupContainers, Labels, Icons, and other controls to change the appearance and behavior of the component.