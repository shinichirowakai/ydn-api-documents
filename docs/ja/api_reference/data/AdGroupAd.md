# AdGroupAd
AdGroupAdオブジェクトは、広告の情報を格納するコンテナです。
### Service
+ [AdGroupAdService](../services/AdGroupAdService.md)

<table>
 <tr>
  <th>Field</th>
  <th>Type</th>
  <th>Description</th>
  <th>response</th>
  <th>get</th>
  <th>add</th>
  <th>set</th>
  <th>remove</th>
 </tr>
 <tr>
  <td>accountId</td>
  <td>xsd:long</td>
  <td>アカウントIDです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Requirement<br>NotUpdatable</td>
  <td>Requirement<br>NotUpdatable</td>
 </tr>
 <tr>
  <td>campaignId</td>
  <td>xsd:long</td>
  <td>キャンペーンIDです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Requirement<br>NotUpdatable</td>
  <td>Requirement<br>NotUpdatable</td>
 </tr>
 <tr>
  <td>campaignName</td>
  <td>xsd:string</td>
  <td>キャンペーン名です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>adGroupId</td>
  <td>xsd:long</td>
  <td>広告グループIDです。 </td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Requirement<br>NotUpdatable</td>
  <td>Requirement<br>NotUpdatable</td>
 </tr> 
 <tr>
  <td>adGroupId</td>
  <td>xsd:string</td>
  <td>広告グループ名です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>adId</td>
  <td>xsd:long</td>
  <td>広告IDです。 </td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>Requirement<br>NotUpdatable</td>
  <td>Requirement<br>NotUpdatable</td>
 </tr>  
 <tr>
  <td>adName</td>
  <td>xsd:string</td>
  <td>広告名です。 </td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>   
 <tr>
  <td>adStyle</td>
  <td>enum <a href="../data/AdStyle.md">AdStyle</a></td>
  <td>掲載フォーマットの種別です。<br>
  ※デフォルト値は「TEXT」</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>mediaId</td>
  <td>xsd:long</td>
  <td>画像IDです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr> 
 <tr>
  <td>userStatus</td>
  <td>enum <a href="../data/UserStatus.md">UserStatus</a></td>
  <td>配信状況です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>  
  <tr>
  <td>approvalStatus</td>
  <td>enum <a href="../data/ApprovalStatus.md">ApprovalStatus</a></td>
  <td>審査状況です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>disapprovalReasonCodes</td>
  <td>xsd:string<br>-num DisapprovalReasonCode</td>
  <td>掲載拒否の理由です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>bid</td>
  <td>AdGroupAdBid<br>inherited <a href="../data/ManualCPCAdGroupAdBid.md">ManualCPCAdGroupAdBid</a></td>
  <td>入札価格です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
 <tr>
  <td>ad</td>
  <td><a href="../data/Ad.md">Ad</a><br>
  inherited <a href="../data/TextAd.md">TextAd</a><br>
  inherited <a href="../data/MobileAd.md">MobileAd</a><br>
  inherited <a href="../data/PosAd.md">PosAd</a><br>
  inherited <a href="../data/ResponsiveAd.md">ResponsiveAd</a><br>
  inherited <a href="../data/StaticFrameAd.md">StaticFrameAd</a><br>
  inherited <a href="../data/None.md">None</a></td>
  <td>広告を含むコンテナです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
 <tr>
  <td>impressionBeaconUrls[0..2]</td>
  <td>xsd:string</td>
  <td>インプレッションビーコンURLです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
 <tr>
  <td>isRemoveBeaconUrls</td>
  <td>enum <a href="../data/isRemoveFlg.md">isRemoveFlg</a></td>
  <td>インプレッションビーコンURL<br>削除フラグです。<br>
  設定値が「TRUE」の場合、設定されている<br>インプレッションビーコンURLの<br>値が無効になります。</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
