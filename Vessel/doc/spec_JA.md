<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
エンティティ船舶  
========<!-- /10-Header -->  
<!-- 15-License -->  
[オープンライセンス](https://github.com/smart-data-models//dataModel.MarineTransport/blob/master/Vessel/LICENSE.md)  
[ドキュメント自動生成](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
グローバルな記述。**このデータモデルは船舶の情報を提供することを目的としている。各船舶の特性（静的、動的情報）を表現することができる**。  
バージョン: 0.0.1  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## プロパティ一覧  

<sup><sub>[*] 属性にタイプがない場合、複数のタイプまたは異なるフォーマット/パターンを持つ可能性があるためです</sub></sup>。  
- `address[object]`: 郵送先住所  . Model: [https://schema.org/address](https://schema.org/address)- `airDraught[number]`: 空気吃水（船舶の最高点から喫水線までの距離）  . Model: [http://schema.org/Number](http://schema.org/Number)- `alternateName[string]`: この項目の別称  - `areaServed[string]`: サービスまたは提供品が提供される地理的な地域  . Model: [https://schema.org/Text](https://schema.org/Text)- `beam[number]`: 船舶のビーム  . Model: [https://schema.org/Number](https://schema.org/Number)- `buildingAt[string]`: ISO 8601 UTCフォーマットで表現された船舶の建造日時。  . Model: [https://schema.org/Text](https://schema.org/Text)- `callSign[string]`: 海上コールサインとは、船舶に固有の識別子として割り当てられるコールサインのことです  . Model: [https://schema.org/Text](https://schema.org/Text)- `courseOverGround[number]`: Course Over Ground（COG）。  . Model: [https://schema.org/Number](https://schema.org/Number)- `createdAt[string]`: ISO 8601 UTCフォーマットで表されるエンティティの作成日時。  . Model: [https://schema.org/Text](https://schema.org/Text)- `dataProvider[string]`: 整合データエンティティの提供者を特定する一連の文字列  . Model: [https://schema.org/Text](https://schema.org/Text)- `dateCreated[string]`: エンティティの作成タイムスタンプ。これは通常、ストレージプラットフォームによって割り当てられる。  - `dateModified[string]`: エンティティの最終更新のタイムスタンプ。これは通常、ストレージプラットフォームによって割り当てられる。  - `deadweightTonnage[number]`: DWT（Deadweight Tonnage）。  . Model: [https://schema.org/Number](https://schema.org/Number)- `description[string]`: このアイテムの説明  - `destinationPort[string]`: 仕向港（地理的コード体系 UN/LOCODE (United Nations Code for Trade and Transport Locations)。https://unece.org/trade/publications/recommendation-ndeg16-united-nations-code-trade-and-transport-locations)  . Model: [https://schema.org/Text](https://schema.org/Text)- `draught[number]`: 喫水線と船底（キール）の垂直距離  . Model: [http://schema.org/Number](http://schema.org/Number)- `financialOwner[string]`: ファイナンシャルオーナー  . Model: [https://schema.org/Text](https://schema.org/Text)- `flagCode[string]`: 国際フラグコード（ISO 3166-1 alfa-2）  . Model: [https://schema.org/Text](https://schema.org/Text)- `grossTonnage[number]`: 総トン数（GT）。  . Model: [https://schema.org/Number](https://schema.org/Number)- `heading[number]`: ヘディング・オブ・ザ・ベッセル（HDG）。  . Model: [https://schema.org/Number](https://schema.org/Number)- `id[string]`: エンティティの一意な識別子  - `imo[number]`: 国際海事機関番号（グローバルな永久UID）  . Model: [https://schema.org/Number](https://schema.org/Number)- `length[number]`: 船舶の長さ  . Model: [https://schema.org/Number](https://schema.org/Number)- `location[object]`: 項目への Geojson リファレンス。Point, LineString, Polygon, MultiPoint, MultiLineString または MultiPolygoProperty とすることができる。  - `manager[string]`: マネージャー・ベッセル  . Model: [https://schema.org/Text](https://schema.org/Text)- `maximumDraught[number]`: 最大喫水。  . Model: [https://schema.org/Number](https://schema.org/Number)- `mmsi[number]`: かいじょうゆうびんばんごう  . Model: [https://schema.org/Number](https://schema.org/Number)- `modifiedAt[string]`: ISO 8601 UTCフォーマットで表されるエンティティの最終更新日時。  . Model: [https://schema.org/Text](https://schema.org/Text)- `name[string]`: 船舶名  . Model: [https://schema.org/Text](https://schema.org/Text)- `navigationStatus[number]`: Enum:0=エンジン使用中,1=停泊中,2=指揮下なし,3=操船制限中,4=喫水制限中,5=係留中,6=停泊中,7=漁業中,8=航海中,9=HSCの航行状態の将来の変更のために保存されます.14=ASCの航行状態の将来の変更のために保存されます,10=Reserved for future amendment of Navigational Status for WIG, 11=Reserved for future use, 12=Reserved for future use, 13=Reserved for future use, 14=AIS-SART is active, 15=Not defined (default)' となる。航行状況。AIVDM/AIVDOのデータフォーマット。  . Model: [http://schema.org/Number](http://schema.org/Number)- `observedAt[string]`: ISO 8601 UTCフォーマットで表現されたこの観測の日付と時刻。  . Model: [https://schema.org/Text](https://schema.org/Text)- `owner[array]`: 所有者の一意のIDを参照するJSONエンコードされた文字列を含むリストです。  - `ownerVessel[string]`: オーナー船  . Model: [https://schema.org/Text](https://schema.org/Text)- `photo[string]`: 船舶写真URL  . Model: [https://schema.org/Text](https://schema.org/Text)- `previousPort[string]`: 旧港（地理的コード体系 UN/LOCODE (United Nations Code for Trade and Transport Locations)。https://unece.org/trade/publications/recommendation-ndeg16-united-nations-code-trade-and-transport-locations)  . Model: [https://schema.org/Text](https://schema.org/Text)- `rateOfTurn[number]`: ROT（Rate of Turn）。  . Model: [https://schema.org/Number](https://schema.org/Number)- `seeAlso[*]`: 項目に関する追加リソースを指すURIのリスト。  - `source[string]`: エンティティデータの元のソースをURLで示す一連の文字。ソースプロバイダの完全修飾ドメイン名、またはソースオブジェクトのURLであることが推奨されます。  - `speedOverGround[number]`: Speed Over Ground（SOG）。  . Model: [https://schema.org/Number](https://schema.org/Number)- `technicalManager[string]`: テクニカルマネージャー  . Model: [https://schema.org/Text](https://schema.org/Text)- `toBow[number]`: Dimension to Bow.  . Model: [http://schema.org/Number](http://schema.org/Number)- `toPort[number]`: ポートまでの寸法。  . Model: [http://schema.org/Number](http://schema.org/Number)- `toStardboard[number]`: スターボードまでの寸法。  . Model: [http://schema.org/Number](http://schema.org/Number)- `toStern[number]`: 寸法は船尾まで。  . Model: [http://schema.org/Number](http://schema.org/Number)- `type[string]`: NGSI Entityタイプ。Vesselである必要があります。  - `vesselSubType[number]`: Enumです。'0=利用不可（デフォルト）,1-19=将来の使用のために保存,20=Wing in Ground (WIG), このタイプのすべての船,21=Wing in Ground (WIG), 危険カテゴリ A,22=Wing in Ground (WIG),危険等級B,23=ウィングイングラウンド（WIG）,危険等級C,24=ウィングイングラウンド（WIG）,危険等級D,25-29=ウィングイングラウンド（WIG）, 将来使用のために予約,30=フィッシング,31=トーイング,32=トーキング:長さ200m超または幅25m超,33=浚渫または水中作業,34=潜水作業,35=軍事作業,36=セーリング,37=プレジャー・クラフト,38-39=予備,40=高速艇(HSC), このタイプの全ての船舶,41=高速艇(HSC), 危険カテゴリA,42=高速艇(HSC), 危険カテゴリB,43=高速艇(HSC), 危険カテゴリC.の船,44=高速艇(HSC)、危険カテゴリD,45-48=高速艇(HSC)、将来の使用のために予約、49=高速艇(HSC)、追加情報なし、50=パイロット船、51=捜索及び救助船、52=タグ、53=ポートテンダー、54=防汚装置、55=法執行、56-57=スペア - ローカル船、58=医療輸送、59=RR決議番号による不戦闘船(Noncombatant Ship according to RR No. 18),60=乗客、60-70=船級士、60-70=船級士、70=船舶,60=船舶,60=船舶,70=船舶のための傭船、70=船舶,70=船舶,70=船舶,90=船舶のための傭船、70=船舶のための傭船18,60=旅客、このタイプの全ての船舶,61=旅客、危険カテゴリA,62=旅客、危険カテゴリB,63=旅客、危険カテゴリC,64=旅客、危険カテゴリD,65-68=旅客、将来の使用のために予約,69=旅客、追加情報なし。70=貨物、このタイプの全ての船舶,71=貨物、危険カテゴリA,72=貨物、危険カテゴリB,73=貨物、危険カテゴリC,74=貨物、危険カテゴリD,75-78=貨物、将来の使用のために予約,79=貨物、追加情報なし,80=タンカー,このタイプの全ての船舶、81=貨物、危険カテゴリC,74=貨物、将来の使用のために予約,90=貨物、追加情報なし、91=貨物、危険カテゴリC,74=貨物,90=貨物,90=タンクトップ,90=タンカー、このタイプの全ての船舶、82=貨物、危険カテゴリC81=タンカー、危険物カテゴリーA、82=タンカー、危険物カテゴリーB、83=タンカー、危険物カテゴリーC、84=タンカー、危険物カテゴリーD、85-88=タンカー、将来の使用のために予約、89=タンカー、追加情報なし、90=その他のタイプ,このタイプのすべての船舶、81=タンカー、危険物カテゴリーD、83=タンカー、危険物カテゴリーD、84=タンカー、追加の情報なし,このタイプのすべての船舶、88=タンカー、将来の使用のために予約、88=タンカー、追加の情報なし、99=その他のタイプ,このタイプのすべての船舶,81=タンカー、危険物カテゴリーA91=その他型、危険物カテゴリーA、92=その他型、危険物カテゴリーB、93=その他型、危険物カテゴリーC、94=その他型、危険物カテゴリーD、95-98=その他型、将来の使用のために予約、99=その他型、追加情報なし'このタイプのすべての船舶。船舶のサブタイプのコード  . Model: [https://schema.org/Number](https://schema.org/Number)- `vesselType[number]`: Enum: '1=Reserved,2=Wing In Ground,3=Special Category,4=High-Speed Craft,5=Special Category,6=Passenger,7=Cargo,8=Tanker,9=Other' です。船舶の種類を表すコード  . Model: [https://schema.org/Number](https://schema.org/Number)- `estimatedTimeOfArrival[string]`: 当初計画され、荷送人が入力した到着予定時刻。  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)- `positionAccuracy[number]`: Enum: '0=Low (> 10 m; GNSS受信機や他の電子位置固定装置の自律モード; デフォルト),1=High (< 10 m; DGNSS受信機などの差分モード)'.船舶位置フラグの精度を表すコード。  . Model: [https://schema.org/Number](https://schema.org/Number)- `specialManeuverIndicator[number]`: Enum: '0=Not available (default),1=Not engaged in special maneuver,2=Engaged in special maneuver'.特殊作戦フラグを表すコード。  . Model: [https://schema.org/Number](https://schema.org/Number)<!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
必要なプロパティ  
- `id`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## プロパティのデータモデル記述  
アルファベット順に並びます（クリックで詳細へ）  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
Vessel:    
  description: 'The data model is intended to provide information about vessels. It allows to represent the properties of each vessel: static and dynamic information'    
  properties:    
    address:    
      description: The mailing address    
      properties:    
        addressCountry:    
          description: 'Property. The country. For example, Spain. Model:''https://schema.org/addressCountry'''    
          type: string    
        addressLocality:    
          description: 'Property. The locality in which the street address is, and which is in the region. Model:''https://schema.org/addressLocality'''    
          type: string    
        addressRegion:    
          description: 'Property. The region in which the locality is, and which is in the country. Model:''https://schema.org/addressRegion'''    
          type: string    
        district:    
          description: 'A district is a type of administrative division that, in some countries, is managed by the local government.'    
          type: string    
        postOfficeBoxNumber:    
          description: 'Property. The post office box number for PO box addresses. For example, 03578. Model:''https://schema.org/postOfficeBoxNumber'''    
          type: string    
        postalCode:    
          description: 'Property. The postal code. For example, 24004. Model:''https://schema.org/https://schema.org/postalCode'''    
          type: string    
        streetAddress:    
          description: 'Property. The street address. Model:''https://schema.org/streetAddress'''    
          type: string    
        streetNr:    
          description: Number identifying a specific property on a public street.    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    airDraught:    
      description: Air Draught (distance from the top of a vessel''s highest point to its waterline)    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    alternateName:    
      description: An alternative name for this item    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: The geographic area where a service or offered item is provided    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    beam:    
      description: Beam of Vessel.    
      maximum: 1000    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' meters'    
    buildingAt:    
      description: Date and time of building of the vessel represented by an ISO 8601 UTC format.    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    callSign:    
      description: Maritime call signs are call signs assigned as unique identifiers to vessels    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    courseOverGround:    
      description: Course Over Ground (COG).    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' degree'    
    createdAt:    
      description: Date and time of creation of the entity represented by an ISO 8601 UTC format.    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    dataProvider:    
      description: A sequence of characters identifying the provider of the harmonised data entity    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    dateCreated:    
      description: Entity creation timestamp. This will usually be allocated by the storage platform.    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    deadweightTonnage:    
      description: Deadweight Tonnage (DWT).    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' tons'    
    description:    
      description: A description of this item    
      type: string    
      x-ngsi:    
        type: Property    
    destinationPort:    
      description: 'Destination Port (Geographic coding scheme UN/LOCODE (United Nations Code for Trade and Transport Locations). https://unece.org/trade/publications/recommendation-ndeg16-united-nations-code-trade-and-transport-locations)'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    draught:    
      description: Draught (vertical distance between the waterline and the bottom of the hull (keel))    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    estimatedTimeOfArrival:    
      description: 'Estimated time of arrival, as it was originally planned and entered by the shipper, represented by an ISO 8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    financialOwner:    
      description: Financial Owner    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    flagCode:    
      description: International Flag Code (ISO 3166-1 alfa-2)    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    grossTonnage:    
      description: Gross Tonnage (GT).    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' moorson tons'    
    heading:    
      description: Heading of the Vessel (HDG).    
      maximum: 511    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' degree'    
    id:    
      description: Unique identifier of the entity    
      type: string    
      x-ngsi:    
        type: Property    
    imo:    
      description: International Maritime Organization Number (a global forever UID)    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    length:    
      description: Length of Vessel.    
      maximum: 8000    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' meters'    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygoProperty.'    
      properties:    
        coordinates:    
          items:    
            type: number    
          type: array    
        type:    
          type: string    
      type: object    
      x-ngsi:    
        type: Geoproperty    
    manager:    
      description: Manager Vessel    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    maximumDraught:    
      description: Maximum Draught.    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' meters'    
    mmsi:    
      description: 'Marine Mobile Service Identity Number (a temporarily assigned UID, issued by that object''s current flag state)'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    modifiedAt:    
      description: Date and time of last modification of the entity represented by an ISO 8601 UTC format.    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    name:    
      description: Vessel Name    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    navigationStatus:    
      description: 'Enum: ''0=Under way using engine,1=At anchor,2=Not under command,3=Restricted manoeuverability,4=Constrained by her draught,5=Moored,6=Aground,7=Engaged in Fishing,8=Under way sailing,9=Reserved for future amendment of Navigational Status for HSC,10=Reserved for future amendment of Navigational Status for WIG,11=Reserved for future use,12=Reserved for future use,13=Reserved for future use,14=AIS-SART is active,15=Not defined (default)''. Navigation Status. AIVDM/AIVDO data format.'    
      enum:    
        - 0    
        - 1    
        - 2    
        - 3    
        - 4    
        - 5    
        - 6    
        - 7    
        - 8    
        - 9    
        - 10    
        - 11    
        - 12    
        - 13    
        - 14    
        - 15    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
    observedAt:    
      description: Date and time of this observation represented by an ISO 8601 UTC format.    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    owner:    
      description: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)    
      items:    
        anyOf:    
          - description: Property. Identifier format of any NGSI entity    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
          - description: Property. Identifier format of any NGSI entity    
            format: uri    
            type: string    
        description: Property. Unique identifier of the entity    
      type: array    
      x-ngsi:    
        type: Property    
    ownerVessel:    
      description: Owner Vessel    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    photo:    
      description: Vessel Photo URL    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    positionAccuracy:    
      description: 'global navigation satellite system (GNSS) receiver or of other electronic position fixing device; default),1=High (< 10 m; differential mode of e.g. DGNSS receiver)''. Code for the accuracy of the vessel position flag.'    
      enum:    
        - 0    
        - 1    
      type: number    
      x-ngsi:    
        model: 'https://schema.org/Number.Enum: 0=Low (> 10 m; autonomous mode of e.g'    
        type: Property    
    previousPort:    
      description: 'Previous Port (Geographic coding scheme UN/LOCODE (United Nations Code for Trade and Transport Locations). https://unece.org/trade/publications/recommendation-ndeg16-united-nations-code-trade-and-transport-locations)'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    rateOfTurn:    
      description: Rate of Turn (ROT).    
      maximum: 708    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' degree'    
    seeAlso:    
      description: list of uri pointing to additional resources about the item    
      oneOf:    
        - items:    
            format: uri    
            type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      x-ngsi:    
        type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: string    
      x-ngsi:    
        type: Property    
    specialManeuverIndicator:    
      description: 'Enum: ''0=Not available (default),1=Not engaged in special maneuver,2=Engaged in special maneuver''. Code for the special maneuver flag.'    
      enum:    
        - 0    
        - 1    
        - 2    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    speedOverGround:    
      description: Speed Over Ground (SOG).    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' meters per second'    
    technicalManager:    
      description: Technical Manager    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    toBow:    
      description: Dimension to Bow.    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    toPort:    
      description: Dimension to Port.    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    toStardboard:    
      description: Dimension to Starboard.    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    toStern:    
      description: Dimension to Stern.    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    type:    
      description: NGSI Entity type. It has to be Vessel    
      enum:    
        - Vessel    
      type: string    
      x-ngsi:    
        type: Property    
    vesselSubType:    
      description: 'Enum: ''0=Not available (default),1-19=Reserved for future use,20=Wing in ground (WIG), all ships of this type,21=Wing in ground (WIG), Hazardous category A,22=Wing in ground (WIG), Hazardous category B,23=Wing in ground (WIG), Hazardous category C,24=Wing in ground (WIG), Hazardous category D,25-29=Wing in ground (WIG), Reserved for future use,30=Fishing,31=Towing,32=Towing: length exceeds 200m or breadth exceeds 25m,33=Dredging or underwater ops,34=Diving ops,35=Military ops,36=Sailing,37=Pleasure Craft,38-39=Reserved,40=High speed craft (HSC), all ships of this type,41=High speed craft (HSC), Hazardous category A,42=High speed craft (HSC), Hazardous category B,43=High speed craft (HSC), Hazardous category C,44=High speed craft (HSC), Hazardous category D,45-48=High speed craft (HSC), Reserved for future use,49=High speed craft (HSC), No additional information,50=Pilot Vessel,51=Search and Rescue vessel,52=Tug,53=Port Tender,54=Anti-pollution equipment,55=Law Enforcement,56-57=Spare - Local Vessel,58=Medical Transport,59=Noncombatant ship according to RR Resolution No. 18,60=Passenger, all ships of this type,61=Passenger, Hazardous category A,62=Passenger, Hazardous category B,63=Passenger, Hazardous category C,64=Passenger, Hazardous category D,65-68=Passenger, Reserved for future use,69=Passenger, No additional information,70=Cargo, all ships of this type,71=Cargo, Hazardous category A,72=Cargo, Hazardous category B,73=Cargo, Hazardous category C,74=Cargo, Hazardous category D,75-78=Cargo, Reserved for future use,79=Cargo, No additional information,80=Tanker, all ships of this type,81=Tanker, Hazardous category A,82=Tanker, Hazardous category B,83=Tanker, Hazardous category C,84=Tanker, Hazardous category D,85-88=Tanker, Reserved for future use,89=Tanker, No additional information,90=Other Type, all ships of this type,91=Other Type, Hazardous category A,92=Other Type, Hazardous category B,93=Other Type, Hazardous category C,94=Other Type, Hazardous category D,95-98=Other Type, Reserved for future use,99=Other Type, no additional information''. Code for vessel Sub-Type'    
      enum:    
        - 1    
        - 2    
        - 3    
        - 4    
        - 5    
        - 6    
        - 7    
        - 8    
        - 9    
        - 10    
        - 11    
        - 12    
        - 13    
        - 14    
        - 15    
        - 16    
        - 17    
        - 18    
        - 19    
        - 20    
        - 21    
        - 22    
        - 23    
        - 24    
        - 25    
        - 26    
        - 27    
        - 28    
        - 29    
        - 30    
        - 31    
        - 32    
        - 33    
        - 34    
        - 35    
        - 36    
        - 37    
        - 38    
        - 39    
        - 40    
        - 41    
        - 42    
        - 43    
        - 44    
        - 45    
        - 46    
        - 47    
        - 48    
        - 49    
        - 50    
        - 51    
        - 52    
        - 53    
        - 54    
        - 55    
        - 56    
        - 57    
        - 58    
        - 59    
        - 60    
        - 61    
        - 62    
        - 63    
        - 64    
        - 65    
        - 66    
        - 67    
        - 68    
        - 69    
        - 70    
        - 71    
        - 72    
        - 73    
        - 74    
        - 75    
        - 76    
        - 77    
        - 78    
        - 79    
        - 80    
        - 81    
        - 82    
        - 83    
        - 84    
        - 85    
        - 86    
        - 87    
        - 88    
        - 89    
        - 90    
        - 91    
        - 92    
        - 93    
        - 94    
        - 95    
        - 96    
        - 97    
        - 98    
        - 99    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    vesselType:    
      description: 'Enum: ''1=Reserved,2=Wing In Ground,3=Special Category,4=High-Speed Craft,5=Special Category,6=Passenger,7=Cargo,8=Tanker,9=Other''. Code for vessel type'    
      enum:    
        - 1    
        - 2    
        - 3    
        - 4    
        - 5    
        - 6    
        - 7    
        - 8    
        - 9    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
  required:    
    - id    
    - type    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2022 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.MarineTransport/blob/master/Vessel/LICENSE.md    
  x-model-schema: https://raw.githubusercontent.com/smart-data-models/dataModel.MarineTransport/master/Vessel/schema.json    
  x-model-tags: I4Trust    
  x-version: 0.0.2    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## ペイロードの例  
#### Vessel NGSI-v2 key-value の例。  
ここでは、VesselをJSON-LD形式でkey-valuesにした例を示します。これは、`options=keyValues`を使用した場合にNGSI-v2と互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:mrn:amura:vessel:test",  
    "type": "Vessel",  
    "location": {  
        "type": "Point",  
        "coordinates": [  
            -5.993307,  
            37.362882  
        ]  
    },  
    "imo": 9863637,  
    "mmsi": 210049000,  
    "callSign": "5BPC5",  
    "name": "ELEANOR ROOSEVELT",  
    "speedOverGround": 1,  
    "courseOverGround": 1,  
    "heading": 1,  
    "rateOfTurn": 1,  
    "createdAt": "2022-06-01T07:00:00.00Z",  
    "modifiedAt": "2022-06-01T07:00:00.00Z",  
    "observedAt": "2022-06-01T07:00:00.00Z",  
    "flagCode": "CY",  
    "vesselType": 1,  
    "vesselSubType": 2,  
    "grossTonnage": 12467,  
    "beam": 7,  
    "length": 32,  
    "maximumDraught": 5,  
    "deadweightTonnage": 8,  
    "buildingAt": "2021-01-01T07:00:00.00Z",  
    "toBow": 3,  
    "toStern": 20,  
    "toPort": 17,  
    "toStardboard": 4,  
    "navigationStatus": 4,  
    "airDraught": 4,  
    "draught": 4,  
    "photo": "PHOTO URL",  
    "ownerVessel": "OWNER NAME",  
    "manager": "MANAGER NAME",  
    "financialOwner": "FINANCIAL OWNER NAME",  
    "technicalManager": "TECHNICAL MANAGER NAME",  
    "dataProvider": "AIS",  
    "destinationPort": "ESVLC",  
    "previousPort": "ESPMI",  
    "estimatedTimeOfArrival": "2023-03-01T07:00:00.00Z",  
    "calculatedTimeOfArrival": "2023-03-02T07:00:00.00Z",  
    "positionAccuracy": 0,  
    "specialManeuverIndicator": 1  
}  
```  
</details>  
#### 容器 NGSI-v2 正規化例  
VesselをJSON-LDフォーマットで正規化した例を示します。これはオプションを使用しない場合、NGSI-v2と互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:mrn:amura:vessel:test",  
    "type": "Vessel",  
    "location": {  
        "type": "geo:json",  
        "value": {  
            "type": "Point",  
            "coordinates": [  
                -5.993307,  
                37.362882  
            ]  
        }  
    },  
    "imo": {  
        "type": "Number",  
        "value": 9863637  
    },  
    "mmsi": {  
        "type": "Number",  
        "value": 210049000  
    },  
    "callSign": {  
        "type": "Text",  
        "value": "5BPC5"  
    },  
    "name": {  
        "type": "Text",  
        "value": "ELEANOR ROOSEVELT"  
    },  
    "speedOverGround": {  
        "type": "Number",  
        "value": 1  
    },  
    "courseOverGround": {  
        "type": "Number",  
        "value": 1  
    },  
    "heading": {  
        "type": "Number",  
        "value": 1  
    },  
    "rateOfTurn": {  
        "type": "Number",  
        "value": 1  
    },  
    "createdAt": {  
        "type": "DateTime",  
        "value": "2022-06-01T07:00:00.00Z"  
    },  
    "modifiedAt": {  
        "type": "DateTime",  
        "value": "2022-06-01T07:00:00.00Z"  
    },  
    "observedAt": {  
        "type": "DateTime",  
        "value": "2022-06-01T07:00:00.00Z"  
    },  
    "flagCode": {  
        "type": "Text",  
        "value": "CY"  
    },  
    "vesselType": {  
        "type": "Number",  
        "value": 1  
    },  
    "vesselSubType": {  
        "type": "Number",  
        "value": 2  
    },  
    "grossTonnage": {  
        "type": "Number",  
        "value": 12467  
    },  
    "beam": {  
        "type": "Number",  
        "value": 7  
    },  
    "length": {  
        "type": "Number",  
        "value": 32  
    },  
    "maximumDraught": {  
        "type": "Number",  
        "value": 5  
    },  
    "deadweightTonnage": {  
        "type": "Number",  
        "value": 8  
    },  
    "buildingAt": {  
        "type": "DateTime",  
        "value": "2021-01-01T07:00:00.00Z1"  
    },  
    "toBow": {  
        "type": "Number",  
        "value": 3  
    },  
    "toStern": {  
        "type": "Number",  
        "value": 20  
    },  
    "toPort": {  
        "type": "Number",  
        "value": 17  
    },  
    "toStardboard": {  
        "type": "Number",  
        "value": 4  
    },  
    "navigationStatus": {  
        "type": "Number",  
        "value": 4  
    },  
    "airDraught": {  
        "type": "Number",  
        "value": 4  
    },  
    "draught": {  
        "type": "Number",  
        "value": 4  
    },  
    "photo": {  
        "type": "Text",  
        "value": "URL PHOTO"  
    },  
    "ownerVessel": {  
        "type": "Text",  
        "value": "OWNER NAME"  
    },  
    "manager": {  
        "type": "Text",  
        "value": "MANAGER NAME"  
    },  
    "financialOwner": {  
        "type": "Text",  
        "value": "FINANCIAL OWNER NAME"  
    },  
    "technicalManager": {  
        "type": "Text",  
        "value": "TECHNICAL MANAGER NAME"  
    },  
    "dataProvider": {  
        "type": "Text",  
        "value": "AIS"  
    },  
    "destinationPort": {  
        "type": "Text",  
        "value": "ESVLC"  
    },  
    "previousPort": {  
        "type": "Text",  
        "value": "ESPMI"  
    },  
    "estimatedTimeOfArrival": {  
        "type": "DateTime",  
        "value": "2023-03-01T07:00:00.00Z"  
    },  
    "positionAccuracy": {  
        "type": "Number",  
        "value": 0  
    },  
    "specialManeuverIndicator": {  
        "type": "Number",  
        "value": 1  
    }  
}  
```  
</details>  
#### 容器NGSI-LDのキー値例  
ここでは、VesselをJSON-LD形式でkey-valuesにした例を示します。これは`options=keyValues`を使用した場合にNGSI-LDと互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:mrn:amura:vessel:test",  
    "type": "Vessel",  
    "location": {  
        "type": "Point",  
        "coordinates": [  
            -5.993307,  
            37.362882  
        ]  
    },  
    "imo": 9863637,  
    "mmsi": 210049000,  
    "callSign": "5BPC5",  
    "name": "ELEANOR ROOSEVELT",  
    "speedOverGround": 1,  
    "courseOverGround": 1,  
    "heading": 1,  
    "rateOfTurn": 1,  
    "createdAt": "2022-06-01T07:00:00.00Z",  
    "modifiedAt": "2022-06-01T07:00:00.00Z",  
    "observedAt": "2022-06-01T07:00:00.00Z",  
    "flagCode": "CY",  
    "vesselType": 1,  
    "vesselSubType": 2,  
    "grossTonnage": 12467,  
    "beam": 7,  
    "length": 32,  
    "maximumDraught": 5,  
    "deadweightTonnage": 8,  
    "buildingAt": "2021-01-01T07:00:00.00Z",  
    "toBow": 3,  
    "toStern": 20,  
    "toPort": 17,  
    "toStardboard": 4,  
    "navigationStatus": 4,  
    "airDraught": 4,  
    "draught": 4,  
    "photo": "PHOTO URL",  
    "ownerVessel": "OWNER NAME",  
    "manager": "MANAGER NAME",  
    "financialOwner": "FINANCIAL OWNER NAME",  
    "technicalManager": "TECHNICAL MANAGER NAME",  
    "dataProvider": "AIS",  
    "destinationPort": "ESVLC",  
    "previousPort": "ESPMI",  
    "estimatedTimeOfArrival": "2023-03-01T07:00:00.00Z",  
    "positionAccuracy": 0,  
    "specialManeuverIndicator": 1,  
    "@context": [  
        "https://gitlab.com/hiades/fiware/smart-data-models/-/raw/main/context.jsonld",  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.MarineTransport/master/context.jsonld"  
    ]  
}  
```  
</details>  
#### NGSI-LDで規格化された容器 例  
VesselをJSON-LD形式で正規化した例です。これはオプションを使用しない場合、NGSI-LDと互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:mrn:amura:vessel:test",  
    "type": "Vessel",  
    "location": {  
        "type": "GeoProperty",  
        "value": {  
            "type": "Point",  
            "coordinates": [  
                -5.993307,  
                37.362882  
            ]  
        }  
    },  
    "imo": {  
        "type": "Property",  
        "value": 9863637  
    },  
    "mmsi": {  
        "type": "Property",  
        "value": 210049000  
    },  
    "callSign": {  
        "type": "Property",  
        "value": "5BPC5"  
    },  
    "name": {  
        "type": "Property",  
        "value": "ELEANOR ROOSEVELT"  
    },  
    "speedOverGround": {  
        "type": "Property",  
        "value": 1  
    },  
    "courseOverGround": {  
        "type": "Property",  
        "value": 1  
    },  
    "heading": {  
        "type": "Property",  
        "value": 1  
    },  
    "rateOfTurn": {  
        "type": "Property",  
        "value": 1  
    },  
    "createdAt": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2022-06-01T07:00:00.00Z"  
        }  
    },  
    "modifiedAt": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2022-06-01T07:00:00.00Z"  
        }  
    },  
    "observedAt": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2022-06-01T07:00:00.00Z"  
        }  
    },  
    "flagCode": {  
        "type": "Property",  
        "value": "CY"  
    },  
    "vesselType": {  
        "type": "Property",  
        "value": 1  
    },  
    "vesselSubType": {  
        "type": "Property",  
        "value": 2  
    },  
    "grossTonnage": {  
        "type": "Property",  
        "value": 12467  
    },  
    "beam": {  
        "type": "Property",  
        "value": 7  
    },  
    "length": {  
        "type": "Property",  
        "value": 32  
    },  
    "maximumDraught": {  
        "type": "Property",  
        "value": 5  
    },  
    "deadweightTonnage": {  
        "type": "Property",  
        "value": 8  
    },  
    "buildingAt": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2021-01-01T07:00:00.00Z1"  
        }  
    },  
    "toBow": {  
        "type": "Property",  
        "value": 3  
    },  
    "toStern": {  
        "type": "Property",  
        "value": 20  
    },  
    "toPort": {  
        "type": "Property",  
        "value": 17  
    },  
    "toStardboard": {  
        "type": "Property",  
        "value": 4  
    },  
    "navigationStatus": {  
        "type": "Property",  
        "value": 4  
    },  
    "airDraught": {  
        "type": "Property",  
        "value": 4  
    },  
    "draught": {  
        "type": "Property",  
        "value": 4  
    },  
    "photo": {  
        "type": "Property",  
        "value": "URL PHOTO"  
    },  
    "ownerVessel": {  
        "type": "Property",  
        "value": "OWNER NAME"  
    },  
    "manager": {  
        "type": "Property",  
        "value": "MANAGER NAME"  
    },  
    "financialOwner": {  
        "type": "Property",  
        "value": "FINANCIAL OWNER NAME"  
    },  
    "technicalManager": {  
        "type": "Property",  
        "value": "TECHNICAL MANAGER NAME"  
    },  
    "dataProvider": {  
        "type": "Property",  
        "value": "AIS"  
    },  
    "destinationPort": {  
        "type": "Property",  
        "value": "ESVLC"  
    },  
    "previousPort": {  
        "type": "Property",  
        "value": "ESPMI"  
    },  
    "estimatedTimeOfArrival": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2023-03-01T07:00:00.00Z"  
        }  
    },  
    "positionAccuracy": {  
        "type": "Property",  
        "value": 0  
    },  
    "specialManeuverIndicator": {  
        "type": "Property",  
        "value": 1  
    },  
    "@context": [  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.MarineTransport/master/context.jsonld"  
    ]  
}  
```  
</details><!-- /80-Examples -->  
<!-- 90-FooterNotes -->  
<!-- /90-FooterNotes -->  
<!-- 95-Units -->  
マグニチュード単位の扱いについては、[FAQ 10](https://smartdatamodels.org/index.php/faqs/)を参照してください。  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
