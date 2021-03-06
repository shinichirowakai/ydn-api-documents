# MediaSelector
MediaSelectorオブジェクトは、操作の対象とする画像およびフィルタ条件を表します。
### Service
+ [MediaService](../services/MediaService.md)

| フィールド | データ型 | 説明 | 
|---|---|---|
| accountId| xsd:long| アカウントIDです。 |
| mediaIds| xsd:long[]| 画像IDです。 |
| userStatus| enum <a href="../data/UserStatus.md">UserStatus[]</a>| 画像の配信の状況です。 |
| approvalStatus| enum <a href="../data/MediaApprovalStatus.md">MediaApprovalStatus[]</a>| 画像の審査の状況です。 |
| paging| <a href="../data/Paging.md">Paging</a>| Paging |
<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
