<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
实体。港口  
=====<!-- /10-Header -->  
<!-- 15-License -->  
[开放许可](https://github.com/smart-data-models//dataModel.MarineTransport/blob/master/Port/LICENSE.md)  
[文件自动生成](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
全局描述。**该数据模型的目的是提供关于端口的信息**。  
版本：0.0.1  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

##属性列表  

<sup><sub>[*] 如果一个属性中没有一个类型，是因为它可能有几种类型或不同的格式/模式</sub></sup>。  
- `address[object]`: 邮寄地址  . Model: [https://schema.org/address](https://schema.org/address)- `alternateName[string]`: 这个项目的一个替代名称  - `areaServed[string]`: 提供服务或提供项目的地理区域  . Model: [https://schema.org/Text](https://schema.org/Text)- `contactPoint[object]`: 与该物品联系的细节。  . Model: [https://schema.org/ContactPoint](https://schema.org/ContactPoint)- `dataProvider[string]`: 一串识别统一数据实体提供者的字符。  - `dateCreated[string]`: 实体创建时间戳。这通常会由存储平台分配。  - `dateModified[string]`: 实体最后一次修改的时间戳。这通常会由存储平台分配。  - `description[string]`: 对这个项目的描述  - `gln[number]`: 全球位置号码。见[GLN](https://gs1id.org/global-location-number-gln)。  . Model: [https://schema.org/Number](https://schema.org/Number)- `id[*]`: 实体的唯一标识符  - `location[*]`: 对该项目的Geojson引用。它可以是点、线字符串、多边形、多点、多线字符串或多多边形。  - `name[string]`: 这个项目的名称。  - `owner[array]`: 一个包含JSON编码的字符序列的列表，引用所有者的唯一Ids。  - `portArea[*]`: GeoProperty。对该项目的Geojson引用。它可以是Polygon或MultiPolygon。  - `portType[string]`: Enum: 'Sea, Inland, Fishing, WarmWater, Dry'.按港口类型分类。  . Model: [http://schema.org/Text](http://schema.org/Text)- `refPortAuthority[*]`: 对PortAuthority的引用  . Model: [https://schema.org/URL](https://schema.org/URL)- `seeAlso[*]`: 指向有关该项目的其他资源的URI列表  - `source[string]`: 一系列字符，以URL的形式给出实体数据的原始来源。建议为源提供者的完全合格域名，或源对象的URL。  - `timeZone[string]`: 所提供的值应属于IANA时区数据库中所列的值。见[时区数据库](https://timezonedb.com/time-zones)。  . Model: [https://schema.org/Text](https://schema.org/Text)- `type[string]`: NGSI实体类型。它必须是端口  - `unlocode[string]`: 联合国贸易和运输地点代码。见[解码](https://unece.org/trade/cefact/unlocode-code-list-country-and-territory)  . Model: [https://schema.org/Text](https://schema.org/Text)<!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
所需属性  
- `id`  - `location`  - `type`  - `unlocode`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## 数据模型的属性描述  
按字母顺序排列（点击查看详情）。  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
Port:    
  description: The data model is intended to provide information about ports    
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
    contactPoint:    
      description: The details to contact with the item.    
      properties:    
        areaServed:    
          description: Property. The geographic area where a service or offered item is provided. Supersedes serviceArea.    
          type: string    
        availabilityRestriction:    
          anyOf:    
            - description: Property. Array of identifiers format of any NGSI entity.    
              items:    
                maxLength: 256    
                minLength: 1    
                pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
                type: string    
              type: array    
            - description: Property. Array of identifiers format of any NGSI entity.    
              items:    
                format: uri    
                type: string    
              type: array    
          description: 'Relationship. Model:''http://schema.org/hoursAvailable''. This property links a contact point to information about when the contact point is not available. The details are provided using the Opening Hours Specification class.'    
        availableLanguage:    
          anyOf:    
            - anyOf:    
                - type: string    
                - items:    
                    type: string    
                  type: array    
          description: 'Property. Model:''http://schema.org/availableLanguage''. A language someone may use with or at the item, service or place. Please use one of the language codes from the IETF BCP 47 standard. It is implemented the Text option but it could be also Language'    
        contactOption:    
          anyOf:    
            - type: string    
            - items:    
                type: string    
              type: array    
          description: 'Property. Model:''http://schema.org/contactOption''. An option available on this contact point (e.g. a toll-free number or support for hearing-impaired callers).'    
        contactType:    
          description: Property. Contact type of this item.    
          type: string    
        email:    
          description: Property. Email address of owner.    
          format: idn-email    
          type: string    
        faxNumber:    
          description: 'Property. Model:''http://schema.org/Text''. The fax number.'    
          type: string    
        name:    
          description: Property. The name of this item.    
          type: string    
        productSupported:    
          description: 'Property. Model:''http://schema.org/Text''. The product or service this support contact point is related to (such as product support for a particular product line). This can be a specific product or product line (e.g. "iPhone") or a general category of products or services (e.g. "smartphones").'    
          type: string    
        telephone:    
          description: Property. Telephone of this contact.    
          type: string    
        url:    
          description: Property. URL which provides a description or further information about this item.    
          format: uri    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/ContactPoint    
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
    gln:    
      description: 'Global Location Number. See [GLN](https://gs1id.org/global-location-number-gln).'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    id:    
      anyOf: &port_-_properties_-_owner_-_items_-_anyof    
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
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: Geoproperty. Geojson reference to the item. Point    
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
        - description: Geoproperty. Geojson reference to the item. LineString    
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
        - description: Geoproperty. Geojson reference to the item. Polygon    
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
        - description: Geoproperty. Geojson reference to the item. MultiPoint    
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
        - description: Geoproperty. Geojson reference to the item. MultiLineString    
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
        - description: Geoproperty. Geojson reference to the item. MultiLineString    
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
        type: Geoproperty    
    name:    
      description: The name of this item.    
      type: string    
      x-ngsi:    
        type: Property    
    owner:    
      description: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)    
      items:    
        anyOf: *port_-_properties_-_owner_-_items_-_anyof    
        description: Property. Unique identifier of the entity    
      type: array    
      x-ngsi:    
        type: Property    
    portArea:    
      description: GeoProperty. Geojson reference to the item. It can be Polygon or MultiPolygon.    
      oneOf:    
        - $id: https://geojson.org/schema/Polygon.json    
          $schema: "http://json-schema.org/draft-07/schema#"    
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
        - $id: https://geojson.org/schema/MultiPolygon.json    
          $schema: "http://json-schema.org/draft-07/schema#"    
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
    portType:    
      description: 'Enum: ''Sea, Inland, Fishing, WarmWater, Dry''. Classification by type of port.'    
      enum:    
        - Dry    
        - Fishing    
        - Inland    
        - Sea    
        - WarmWater    
      type: string    
      x-ngsi:    
        model: http://schema.org/Text    
        type: Property    
    refPortAuthority:    
      anyOf:    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Reference to the PortAuthority    
      x-ngsi:    
        model: https://schema.org/URL    
        type: Relationship    
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
    timeZone:    
      description: 'The value provided should be among those listed in the IANA Time Zone Database. See [Time Zone Database](https://timezonedb.com/time-zones).'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    type:    
      description: NGSI Entity type. It has to be Port    
      enum:    
        - Port    
      type: string    
      x-ngsi:    
        type: Property    
    unlocode:    
      description: 'United Nations Code for Trade and Transport Locations. See [Unlocode](https://unece.org/trade/cefact/unlocode-code-list-country-and-territory)'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
  required:    
    - id    
    - type    
    - location    
    - unlocode    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2022 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.MarineTransport/blob/master/Port/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/dataModel.Ports/Port/schema.json    
  x-model-tags: ""    
  x-version: 0.0.1    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## ＃＃＃＃有效载荷的例子  
#### 端口NGSI-v2密钥值示例  
这里是一个以JSON-LD格式作为key-values的Port的例子。当使用`options=keyValues`时，这与NGSI-v2兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:mrn:amura:port:UNLOCODE",  
  "type": "Port",  
  "location": {  
      "type": "Point",  
      "coordinates": [  
          -0.3048254137983776,  
          39.431348987126704  
      ]  
  },  
  "name": "Port name",  
  "unlocode": "Unlocode",  
  "description": "Port description",  
  "address": {  
    "streetAddress": "Avda. Example",  
      "addressCountry": "ES",  
      "addressLocality": "Locality",  
      "postalCode": "1234"  
  },  
  "contactPoint": {  
    "telephone": "+34 12 34 56 78",  
    "email": "example@port.com",  
    "availableLanguage": [  
      "en-EN",  
      "es-ES"  
    ],  
    "faxNumber": "12 345 67 89",  
    "name": "Portname",  
    "url": "https://URL"  
  },  
  "portArea": {  
    "type": "MultiPolygon",  
    "coordinates": [  
      [  
        [  
          [  
            -0.33295074395914526,  
            39.4631637203228  
          ],  
          [  
            -0.33295074395914526,  
            39.42053808578652  
          ],  
          [  
            -0.2829300303054083,  
            39.42053808578652  
          ],  
          [  
            -0.2829300303054083,  
            39.4631637203228  
          ],  
          [  
            -0.33295074395914526,  
            39.4631637203228  
          ]  
        ]  
      ]  
    ]  
  },  
  "timeZone": "Europe/London",  
  "gln":  123456789,  
  "portType": "Sea",  
  "refPortAuthority": "urn:mrn:amura:port-authority:UNLOCODE"  
}  
```  
</details>  
#### 端口NGSI-v2规范化示例  
下面是一个规范化的JSON-LD格式的Port的例子。当不使用选项时，这与NGSI-v2兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:mrn:amura:port:UNLOCODE",  
  "type": "Port",  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
          -0.3048254137983776,  
          39.431348987126704  
      ]  
    }  
  },  
  "name": {  
      "type": "Text",  
      "value": "Port name"  
  },  
  "unlocode": {  
    "type": "Text",  
    "value": "Unlocode"  
  },  
  "description": {  
    "type": "Text",  
    "value": "Port description"  
  },  
  "address": {  
    "type": "StructuredValue",  
    "value": {  
      "streetAddress": "Avda. Example",  
      "addressCountry": "ES",  
      "addressLocality": "Locality",  
      "postalCode": "1234"  
    }  
  },  
  "contactPoint": {  
    "type": "StructuredValue",  
    "value": {  
      "telephone": "+34 12 34 56 78",  
      "email": "example@port.com",  
      "availableLanguage": [  
        "en-EN",  
        "es-ES"  
      ],  
      "faxNumber": "12 345 67 89",  
      "name": "Portname",  
      "url": "https://URL"  
    }  
  },  
  "portArea":{  
    "type": "geo:json",  
    "value": {  
      "type": "MultiPolygon",  
      "coordinates": [  
        [  
          [  
            [  
              -0.33295074395914526,  
              39.4631637203228  
            ],  
            [  
              -0.33295074395914526,  
              39.42053808578652  
            ],  
            [  
              -0.2829300303054083,  
              39.42053808578652  
            ],  
            [  
              -0.2829300303054083,  
              39.4631637203228  
            ],  
            [  
              -0.33295074395914526,  
              39.4631637203228  
            ]  
          ]  
        ]  
      ]  
    }  
  },  
  "timeZone": {  
    "type": "Text",  
    "value": "Europe/London"  
  },  
  "gln": {  
    "type": "Number",  
    "value": 123456789  
  },  
  "portType": {  
    "type": "Text",  
    "value": "Sea"  
  },  
  "refPortAuthority": {  
      "type": "Reference",  
      "value": "urn:mrn:amura:port-authority:UNLOCODE"  
  }  
}  
```  
</details>  
#### 端口NGSI-LD密钥值示例  
这里是一个以JSON-LD格式作为key-values的Port的例子。当使用`options=keyValues`时，这与NGSI-LD兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:mrn:amura:port:UNLOCODE",  
  "type": "Port",  
  "location": {  
      "type": "Point",  
      "coordinates": [  
          -0.3048254137983776,  
          39.431348987126704  
      ]  
  },  
  "name": "Port name",  
  "unlocode": "Unlocode",  
  "description": "Port description",  
  "address": {  
    "streetAddress": "Avda. Example",  
      "addressCountry": "ES",  
      "addressLocality": "Locality",  
      "postalCode": "1234"  
  },  
  "contactPoint": {  
    "telephone": "+34 12 34 56 78",  
    "email": "example@port.com",  
    "availableLanguage": [  
      "en-EN",  
      "es-ES"  
    ],  
    "faxNumber": "12 345 67 89",  
    "name": "Portname",  
    "url": "https://URL"  
  },  
  "portArea": {  
    "type": "MultiPolygon",  
    "coordinates": [  
      [  
        [  
          [  
            -0.33295074395914526,  
            39.4631637203228  
          ],  
          [  
            -0.33295074395914526,  
            39.42053808578652  
          ],  
          [  
            -0.2829300303054083,  
            39.42053808578652  
          ],  
          [  
            -0.2829300303054083,  
            39.4631637203228  
          ],  
          [  
            -0.33295074395914526,  
            39.4631637203228  
          ]  
        ]  
      ]  
    ]  
  },  
  "timeZone": "Europe/London",  
  "gln":  123456789,  
  "portType": "Sea",  
  "refPortAuthority": "urn:mrn:amura:port-authority:UNLOCODE",  
  "@context": [  
    "https://gitlab.com/hiades/fiware/smart-data-models/-/raw/main/context.jsonld"  
  ]  
}  
```  
</details>  
#### 端口NGSI-LD规范化示例  
下面是一个规范化的JSON-LD格式的Port的例子。当不使用选项时，这与NGSI-LD兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:mrn:amura:port:UNLOCODE",  
  "type": "Port",  
  "location": {  
    "type": "GeoProperty",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
          -0.3048254137983776,  
          39.431348987126704  
      ]  
    }  
  },  
  "name": {  
      "type": "Property",  
      "value": "Port name"  
  },  
  "unlocode": {  
    "type": "Property",  
    "value": "Unlocode"  
  },  
  "description": {  
    "type": "Property",  
    "value": "Port description"  
  },  
  "address": {  
    "type": "Property",  
    "value": {  
      "streetAddress": "Avda. Example",  
      "addressCountry": "ES",  
      "addressLocality": "Locality",  
      "postalCode": "1234"  
    }  
  },  
  "contactPoint": {  
    "type": "Property",  
    "value": {  
      "telephone": "+34 12 34 56 78",  
      "email": "example@port.com",  
      "availableLanguage": [  
        "en-EN",  
        "es-ES"  
      ],  
      "faxProperty": "12 345 67 89",  
      "name": "Portname",  
      "url": "https://URL"  
    }  
  },  
  "portArea":{  
    "type": "GeoProperty",  
    "value": {  
      "type": "MultiPolygon",  
      "coordinates": [  
        [  
          [  
            [  
              -0.33295074395914526,  
              39.4631637203228  
            ],  
            [  
              -0.33295074395914526,  
              39.42053808578652  
            ],  
            [  
              -0.2829300303054083,  
              39.42053808578652  
            ],  
            [  
              -0.2829300303054083,  
              39.4631637203228  
            ],  
            [  
              -0.33295074395914526,  
              39.4631637203228  
            ]  
          ]  
        ]  
      ]  
    }  
  },  
  "timeZone": {  
    "type": "Property",  
    "value": "Europe/London"  
  },  
  "gln": {  
    "type": "Property",  
    "value": 123456789  
  },  
  "portType": {  
    "type": "Property",  
    "value": "Sea"  
  },  
  "refPortAuthority": {  
      "type": "Relationship",  
      "value": "urn:mrn:amura:port-authority:UNLOCODE"  
  },  
  "@context": [  
    "https://gitlab.com/hiades/fiware/smart-data-models/-/raw/main/context.jsonld"  
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
