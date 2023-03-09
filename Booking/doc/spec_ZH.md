<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
实体。预订  
=====<!-- /10-Header -->  
<!-- 15-License -->  
[开放许可](https://github.com/smart-data-models//dataModel.MarineTransport/blob/master/Booking/LICENSE.md)  
[文件自动生成](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
全球描述。**提供预订的电子信息描述**。  
版本：0.0.1  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

##属性列表  

<sup><sub>[*] 如果一个属性中没有一个类型，是因为它可能有几种类型或不同的格式/模式</sub></sup>。  
- `actualWindowFrom[number]`: 实际使用的时间窗口，如果到达时间提前15'的话  - `actualWindowTo[number]`: 实际使用的时间窗口  - `address[object]`: 邮寄地址  . Model: [https://schema.org/address](https://schema.org/address)- `alternateName[string]`: 这个项目的一个替代名称  - `areaServed[string]`: 提供服务或提供项目的地理区域  . Model: [https://schema.org/Text](https://schema.org/Text)- `bookingDate[number]`: 预订日期  - `bookingNumber[number]`: 预订的唯一ID  - `bookingStatus[string]`: 预订情况  - `company[string]`: 预订的公司  - `containersExport[number]`: 从CT堆场提取的集装箱数量  - `containersImport[number]`: 投放到CT场的集装箱数量  - `dataProvider[string]`: 一串识别统一数据实体提供者的字符。  - `dateCreated[string]`: 实体创建时间戳。这通常会由存储平台分配。  - `dateModified[string]`: 实体最后一次修改的时间戳。这通常会由存储平台分配。  - `description[string]`: 对这个项目的描述  - `enterDate[number]`: 实际进入的时间  - `exportContainer1[string]`: 第一个被取走的集装箱的独特的集装箱ID  - `exportContainer2[string]`: 第2个被取走的集装箱的独特集装箱ID  - `id[*]`: 实体的唯一标识符  - `importContainer1[string]`: 第一个被丢弃的集装箱的独特的集装箱ID  - `importContainer2[string]`: 第2个被丢弃的集装箱的独特集装箱ID  - `location[*]`: 对该项目的Geojson引用。它可以是点、线字符串、多边形、多点、多线字符串或多多边形。  - `name[string]`: 这个项目的名称。  - `originalWindowFrom[number]`: 原先预订的进入时间窗口  - `originalWindowTo[number]`: 最初估计离开的时间窗口  - `owner[array]`: 一个包含JSON编码的字符序列的列表，引用所有者的唯一Ids。  - `seeAlso[*]`: 指向有关该项目的其他资源的URI列表  - `source[string]`: 提供实体数据原始来源的一连串字符，作为一个URL。建议为源提供者的完全合格域名，或源对象的URL。  - `windowDate[number]`: 时间窗口的日期  <!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
所需属性  
- `id`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
将卡车的尺寸限制在两个集装箱内，证明其属性为1和2。  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## 数据模型的属性描述  
按字母顺序排列（点击查看详情）。  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
Booking:    
  description: Provide the bookings electronic messaging description    
  properties:    
    actualWindowFrom:    
      description: 'Time window actually used, if arrival was 15’ earlier'    
      type: number    
      x-ngsi:    
        type: Property    
    actualWindowTo:    
      description: Time window actually used    
      type: number    
      x-ngsi:    
        type: Property    
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
    bookingDate:    
      description: Booking date    
      type: number    
      x-ngsi:    
        type: Property    
    bookingNumber:    
      description: Unique ID of the booking    
      type: number    
      x-ngsi:    
        type: Property    
    bookingStatus:    
      description: Booking status    
      enum:    
        - Pending    
        - No show    
        - Visited    
        - Cancelled by user (on time)    
        - No-slot booking    
      type: string    
      x-ngsi:    
        type: Property    
    company:    
      description: Company making the booking    
      type: string    
      x-ngsi:    
        type: Property    
    containersExport:    
      description: Number of containers to pick-up from the CT yard    
      maximum: 2    
      minimum: 0    
      type: number    
      x-ngsi:    
        type: Property    
    containersImport:    
      description: Number of containers to drop-off to the CT yard    
      maximum: 2    
      minimum: 0    
      type: number    
      x-ngsi:    
        type: Property    
    dataProvider:    
      description: A sequence of characters identifying the provider of the harmonised data entity.    
      type: string    
      x-ngsi:    
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
    description:    
      description: A description of this item    
      type: string    
      x-ngsi:    
        type: Property    
    enterDate:    
      description: Actual time of entering    
      type: number    
      x-ngsi:    
        type: Property    
    exportContainer1:    
      description: Unique container ID for 1st container to be picked-up    
      type: string    
      x-ngsi:    
        type: Property    
    exportContainer2:    
      description: Unique container ID for 2nd container to be picked-up    
      type: string    
      x-ngsi:    
        type: Property    
    id:    
      anyOf: &booking_-_properties_-_owner_-_items_-_anyof    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Unique identifier of the entity    
      x-ngsi:    
        type: Property    
    importContainer1:    
      description: Unique container ID for 1st container to be dropped-off    
      type: string    
      x-ngsi:    
        type: Property    
    importContainer2:    
      description: Unique container ID for 2nd container to be dropped-off    
      type: string    
      x-ngsi:    
        type: Property    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: GeoProperty. Geojson reference to the item. Point    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                type: number    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - Point    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Point    
          type: object    
        - description: GeoProperty. Geojson reference to the item. LineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - LineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON LineString    
          type: object    
        - description: GeoProperty. Geojson reference to the item. Polygon    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 4    
                type: array    
              type: array    
            type:    
              enum:    
                - Polygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Polygon    
          type: object    
        - description: GeoProperty. Geojson reference to the item. MultiPoint    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPoint    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPoint    
          type: object    
        - description: GeoProperty. Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiLineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiLineString    
          type: object    
        - description: GeoProperty. Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    items:    
                      type: number    
                    minItems: 2    
                    type: array    
                  minItems: 4    
                  type: array    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPolygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPolygon    
          type: object    
      x-ngsi:    
        type: GeoProperty    
    name:    
      description: The name of this item.    
      type: string    
      x-ngsi:    
        type: Property    
    originalWindowFrom:    
      description: Originally booked time window to enter    
      type: number    
      x-ngsi:    
        type: Property    
    originalWindowTo:    
      description: Originally estimated time window to leave    
      type: number    
      x-ngsi:    
        type: Property    
    owner:    
      description: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)    
      items:    
        anyOf: *booking_-_properties_-_owner_-_items_-_anyof    
        description: Property. Unique identifier of the entity    
      type: array    
      x-ngsi:    
        type: Property    
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
    windowDate:    
      description: Date of the time window    
      type: number    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2022 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.MarineTransport/blob/master/Booking/LICENSE.md    
  x-model-schema: https://github.com/smart-data-models/dataModel.MarineTransport/master/Booking/schema.json    
  x-model-tags: ""    
  x-version: 0.0.1    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## ＃＃＃＃有效载荷的例子  
#### 预订NGSI-v2密钥值的例子  
这里是一个以JSON-LD格式作为key-values的Booking的例子。当使用`options=keyValues`时，这与NGSI-v2兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:ThPA:Booking:463589473290389",  
  "type": "Booking",  
  "bookingNumber": 463589473290389,  
  "bookingDate": 20220621,  
  "company": "Pantelis Bouratsis",  
  "enterDate": 2021,  
  "originalWindowFrom": 660,  
  "actualWindowFrom": 645,  
  "originalWindowTo": 720,  
  "actualWindowTo": 960,  
  "windowDate": 20220621,  
  "bookingStatus": "Pending",  
  "containersImport": 1,  
  "containersExport": 2,  
  "exportContainer1": "",  
  "exportContainer2": "",  
  "importContainer1": "ZCSU7627029",  
  "importContainer2": ""  
}  
```  
</details>  
#### 预订NGSI-v2规范化示例  
下面是一个以JSON-LD格式规范化的Booking的例子。当不使用选项时，这与NGSI-v2兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:ThPA:Booking:463589473290389",  
  "type": "Booking",  
  "actualWindowFrom": {  
    "type": "Number",  
    "value": 645,  
    "metadata": {}  
  },  
  "actualWindowTo": {  
    "type": "Number",  
    "value": 960,  
    "metadata": {}  
  },  
  "bookingDate": {  
    "type": "Text",  
    "value": "20220621",  
    "metadata": {}  
  },  
  "bookingNumber": {  
    "type": "Text",  
    "value": "463589473290389",  
    "metadata": {}  
  },  
  "bookingStatus": {  
    "type": "Text",  
    "value": "Pending",  
    "metadata": {}  
  },  
  "company": {  
    "type": "Text",  
    "value": "Pantelis Bouratsis",  
    "metadata": {}  
  },  
  "containersExport": {  
    "type": "Number",  
    "value": 0,  
    "metadata": {}  
  },  
  "containersImport": {  
    "type": "Number",  
    "value": 1,  
    "metadata": {}  
  },  
  "exportContainer1": {  
    "type": "Text",  
    "value": "",  
    "metadata": {}  
  },  
  "exportContainer2": {  
    "type": "Text",  
    "value": "",  
    "metadata": {}  
  },  
  "importContainer1": {  
    "type": "Text",  
    "value": "ZCSU7627029",  
    "metadata": {}  
  },  
  "importContainer2": {  
    "type": "Text",  
    "value": "",  
    "metadata": {}  
  },  
  "originalWindowFrom": {  
    "type": "Number",  
    "value": 660,  
    "metadata": {}  
  },  
  "originalWindowTo": {  
    "type": "Number",  
    "value": 720,  
    "metadata": {}  
  },  
  "windowDate": {  
    "type": "Text",  
    "value": "20220621",  
    "metadata": {}  
  }  
}  
```  
</details>  
#### 预订NGSI-LD的关键值示例  
这里是一个以JSON-LD格式作为key-values的Booking的例子。当使用`options=keyValues`时，这与NGSI-LD兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:ThPA:Booking:463589473290389",  
  "type": "Booking",  
  "bookingNumber": 463589473290389,  
  "bookingDate": 20220621,  
  "company": "Pantelis Bouratsis",  
  "enterDate": 2021,  
  "originalWindowFrom": 660,  
  "actualWindowFrom": 645,  
  "originalWindowTo": 720,  
  "actualWindowTo": 960,  
  "windowDate": 20220621,  
  "bookingStatus": "Pending",  
  "containersImport": 1,  
  "containersExport": 2,  
  "exportContainer1": "",  
  "exportContainer2": "",  
  "importContainer1": "ZCSU7627029",  
  "importContainer2": "",  
  "@context": [  
    "https://raw.githubusercontent.com/smart-data-models/dataModel.MarineTransport/master/context.jsonld"  
  ]  
}  
```  
</details>  
#### 预订NGSI-LD正常化的例子  
这里是一个以JSON-LD格式规范化的Booking的例子。当不使用选项时，这与NGSI-LD兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:ThPA:Booking:463589473290389",  
  "type": "Booking",  
  "actualWindowFrom": {  
    "type": "Property",  
    "value": 645  
  },  
  "actualWindowTo": {  
    "type": "Property",  
    "value": 960  
  },  
  "bookingDate": {  
    "type": "Property",  
    "value": "20220621"  
  },  
  "bookingProperty": {  
    "type": "Property",  
    "value": "463589473290389"  
  },  
  "bookingStatus": {  
    "type": "Property",  
    "value": "Pending"  
  },  
  "company": {  
    "type": "Property",  
    "value": "Pantelis Bouratsis"  
  },  
  "containersExport": {  
    "type": "Property",  
    "value": 0  
  },  
  "containersImport": {  
    "type": "Property",  
    "value": 1  
  },  
  "exportContainer1": {  
    "type": "Property",  
    "value": ""  
  },  
  "exportContainer2": {  
    "type": "Property",  
    "value": ""  
  },  
  "importContainer1": {  
    "type": "Property",  
    "value": "ZCSU7627029"  
  },  
  "importContainer2": {  
    "type": "Property",  
    "value": ""  
  },  
  "originalWindowFrom": {  
    "type": "Property",  
    "value": 660  
  },  
  "originalWindowTo": {  
    "type": "Property",  
    "value": 720  
  },  
  "windowDate": {  
    "type": "Property",  
    "value": "20220621"  
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
参见[常见问题10](https://smartdatamodels.org/index.php/faqs/)，以获得关于如何处理量级单位的答案。  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
