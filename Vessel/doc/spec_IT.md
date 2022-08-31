[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
Entità: Nave  
============  
[Licenza aperta](https://github.com/smart-data-models//dataModel.MarineTransport/blob/master/Vessel/LICENSE.md)  
[documento generato automaticamente](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
Descrizione globale: **Il modello di dati è destinato a fornire informazioni sulle imbarcazioni. Permette di rappresentare le proprietà di ogni imbarcazione: informazioni statiche e dinamiche**  
versione: 0.0.1  

## Elenco delle proprietà  

- `address`: L'indirizzo postale  - `airDraught`: Pescaggio dell'aria (distanza tra il punto più alto di una nave e la sua linea di galleggiamento)  - `alternateName`: Un nome alternativo per questa voce  - `areaServed`: L'area geografica in cui viene fornito il servizio o l'articolo offerto.  - `beam`: Larghezza della nave.  - `buildingAt`: Data e ora di costruzione dell'imbarcazione rappresentate in formato ISO 8601 UTC.  - `callSign`: I nominativi marittimi sono nominativi assegnati come identificativi univoci alle navi.  - `courseOverGround`: Rotta sul terreno (COG).  - `createdAt`: Data e ora di creazione dell'entità rappresentata da un formato ISO 8601 UTC.  - `dataProvider`: una sequenza di caratteri che identifica il fornitore dell'entità di dati armonizzati  - `dateCreated`: Timestamp di creazione dell'entità. Di solito viene assegnato dalla piattaforma di archiviazione.  - `dateModified`: Timestamp dell'ultima modifica dell'entità. Di solito viene assegnato dalla piattaforma di archiviazione.  - `deadweightTonnage`: Tonnellata di portata lorda (DWT).  - `description`: Descrizione dell'articolo  - `destinationPort`: Porto di destinazione (schema di codifica geografica UN/LOCODE (Codice delle Nazioni Unite per le località di commercio e trasporto). https://unece.org/trade/publications/recommendation-ndeg16-united-nations-code-trade-and-transport-locations)  - `draught`: Pescaggio (distanza verticale tra la linea di galleggiamento e il fondo dello scafo (chiglia))  - `financialOwner`: Proprietario finanziario  - `flagCode`: Codice internazionale delle bandiere (ISO 3166-1 alfa-2)  - `grossTonnage`: Stazza lorda (GT).  - `heading`: Direzione della nave (HDG).  - `id`: Identificatore univoco dell'entità  - `imo`: Numero dell'Organizzazione Marittima Internazionale (un UID globale per sempre)  - `length`: Lunghezza della nave.  - `location`: Riferimento Geojson all'elemento. Può essere un punto, una stringa di linea, un poligono, un multi-punto, una stringa di linea o una proprietà multi-poligono.  - `manager`: Manager Vessel  - `maximumDraught`: Pescaggio massimo.  - `mmsi`: Marine Mobile Service Identity Number (un UID temporaneamente assegnato, emesso dall'attuale stato di bandiera dell'oggetto)  - `modifiedAt`: Data e ora dell'ultima modifica dell'entità rappresentata da un formato ISO 8601 UTC.  - `name`: Nome della nave  - `navigationStatus`: Enum: '0=In navigazione con motore,1=Ancora,2=Non sotto comando,3=Manovrabilità limitata,4=Costretta dal pescaggio,5=Ormeggiata,6=Interrata,7=Impegnata nella pesca,8=In navigazione,9=Riservata per future modifiche dello stato di navigazione per HSC,10=Riservato per future modifiche dello stato di navigazione per WIG,11=Riservato per uso futuro,12=Riservato per uso futuro,13=Riservato per uso futuro,14=AIS-SART attivo,15=Non definito (default)". Stato della navigazione. Formato dati AIVDM/AIVDO.  - `observedAt`: Data e ora di questa osservazione rappresentate in formato ISO 8601 UTC.  - `owner`: Un elenco contenente una sequenza di caratteri codificata JSON che fa riferimento agli ID univoci dei proprietari.  - `ownerVessel`: Proprietario dell'imbarcazione  - `photo`: URL della foto della nave  - `previousPort`: Porto precedente (schema di codifica geografica UN/LOCODE (Codice delle Nazioni Unite per le località di commercio e trasporto). https://unece.org/trade/publications/recommendation-ndeg16-united-nations-code-trade-and-transport-locations)  - `rateOfTurn`: Velocità di rotazione (ROT).  - `seeAlso`: elenco di uri che puntano a risorse aggiuntive sull'elemento  - `source`: Una sequenza di caratteri che indica la fonte originale dei dati dell'entità come URL. Si consiglia di utilizzare il nome di dominio completamente qualificato del provider di origine o l'URL dell'oggetto di origine.  - `speedOverGround`: Velocità sul terreno (SOG).  - `technicalManager`: Responsabile tecnico  - `toBow`: Dimensione a prua.  - `toPort`: Dimensioni alla porta.  - `toStardboard`: Dimensione a dritta.  - `toStern`: Dimensione a poppa.  - `type`: Tipo di entità NGSI. Deve essere Vessel  - `vesselSubType`: Enum: '0=Non disponibile (default),1-19=Riservato per uso futuro,20=Aletta a terra (WIG), tutte le navi di questo tipo,21=Aletta a terra (WIG), categoria pericolosa A,22=Aletta a terra (WIG), Pericolosa categoria B,23=Aletta a terra (WIG), Pericolosa categoria C,24=Aletta a terra (WIG), Pericolosa categoria D,25-29=Aletta a terra (WIG), Riservato per uso futuro,30=Pesca,31=Trattori,32=Trattori: lunghezza superiore a 200 m o larghezza superiore a 25 m,33=Dragaggio o operazioni subacquee,34=Operazioni subacquee,35=Operazioni militari,36=Vela,37=Imbarcazioni da diporto,38-39=Riservato,40=Imbarcazioni ad alta velocità (HSC), tutte le navi di questo tipo,41=Imbarcazioni ad alta velocità (HSC), categoria pericolosa A,42=Imbarcazioni ad alta velocità (HSC), categoria pericolosa B,43=Imbarcazioni ad alta velocità (HSC), categoria pericolosa C,44=Autoveicolo ad alta velocità (HSC), categoria pericolosa D,45-48=Autoveicolo ad alta velocità (HSC), riservato per uso futuro,49=Autoveicolo ad alta velocità (HSC), nessuna informazione aggiuntiva,50=nave pilota,51=nave per ricerca e soccorso,52=rimorchiatore,53=tender portuale,54=attrezzatura antinquinamento,55=vigilanza,56-57=nave di riserva - locale,58=trasporto medico,59=nave non combattente secondo la risoluzione RR n. 18,60=nave passeggeri,60=nave per il trasporto di persone. 18,60=Passeggeri, tutte le navi di questo tipo,61=Passeggeri, categoria pericolosa A,62=Passeggeri, categoria pericolosa B,63=Passeggeri, categoria pericolosa C,64=Passeggeri, categoria pericolosa D,65-68=Passeggeri, Riservato per uso futuro,69=Passeggeri, Nessuna informazione aggiuntiva,70=Cargo, tutte le navi di questo tipo,71=Cargo, categoria pericolosa A,72=Cargo, categoria pericolosa B,73=Cargo, categoria pericolosa C,74=Cargo, categoria pericolosa D,75-78=Cargo, Riservato per usi futuri,79=Cargo, Nessuna informazione aggiuntiva,80=Cisterna, tutte le navi di questo tipo,81=Cisterna, categoria pericolosa A,82=Cisterna, categoria pericolosa B,83=Cisterna, categoria pericolosa C,84=Cisterna, categoria pericolosa D,85-88=Cisterna, Riservato per usi futuri,89=Cisterna, Nessuna informazione aggiuntiva,90=Altro tipo, tutte le navi di questo tipo,91=Altro tipo, categoria pericolosa A,92=Altro tipo, categoria pericolosa B,93=Altro tipo, categoria pericolosa C,94=Altro tipo, categoria pericolosa D,95-98=Altro tipo, riservato per uso futuro,99=Altro tipo, nessuna informazione aggiuntiva". Codice del sottotipo di nave  - `vesselType`: Enum: "1=Riservato,2=Aeromobile a terra,3=Categoria speciale,4=Imbarcazione ad alta velocità,5=Categoria speciale,6=Passeggeri,7=Cargo,8=Cisterna,9=Altro". Codice del tipo di nave    
Proprietà richieste  
- `id`  - `type`  ## Modello di dati descrizione delle proprietà  
Ordinati in ordine alfabetico (clicca per i dettagli)  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
Vessel:    
  description: 'The data model is intended to provide information about vessels. It allows to represent the properties of each vessel: static and dynamic information'    
  properties:    
    address:    
      description: 'The mailing address'    
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
        postOfficeBoxNumber:    
          description: 'Property. The post office box number for PO box addresses. For example, 03578. Model:''https://schema.org/postOfficeBoxNumber'''    
          type: string    
        postalCode:    
          description: 'Property. The postal code. For example, 24004. Model:''https://schema.org/https://schema.org/postalCode'''    
          type: string    
        streetAddress:    
          description: 'Property. The street address. Model:''https://schema.org/streetAddress'''    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    airDraught:    
      description: 'Air Draught (distance from the top of a vessel''''s highest point to its waterline)'    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    alternateName:    
      description: 'An alternative name for this item'    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: 'The geographic area where a service or offered item is provided'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    beam:    
      description: 'Beam of Vessel.'    
      maximum: 1000    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' meters'    
    buildingAt:    
      description: 'Date and time of building of the vessel represented by an ISO 8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    callSign:    
      description: 'Maritime call signs are call signs assigned as unique identifiers to vessels'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    courseOverGround:    
      description: 'Course Over Ground (COG).'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' degree'    
    createdAt:    
      description: 'Date and time of creation of the entity represented by an ISO 8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    dataProvider:    
      description: 'A sequence of characters identifying the provider of the harmonised data entity'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    dateCreated:    
      description: 'Entity creation timestamp. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: 'Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    deadweightTonnage:    
      description: 'Deadweight Tonnage (DWT).'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' tons'    
    description:    
      description: 'A description of this item'    
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
      description: 'Draught (vertical distance between the waterline and the bottom of the hull (keel))'    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    financialOwner:    
      description: 'Financial Owner'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    flagCode:    
      description: 'International Flag Code (ISO 3166-1 alfa-2)'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    grossTonnage:    
      description: 'Gross Tonnage (GT).'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' moorson tons'    
    heading:    
      description: 'Heading of the Vessel (HDG).'    
      maximum: 511    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' degree'    
    id:    
      description: 'Unique identifier of the entity'    
      type: string    
      x-ngsi:    
        type: Property    
    imo:    
      description: 'International Maritime Organization Number (a global forever UID)'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    length:    
      description: 'Length of Vessel.'    
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
      description: 'Manager Vessel'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    maximumDraught:    
      description: 'Maximum Draught.'    
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
      description: 'Date and time of last modification of the entity represented by an ISO 8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    name:    
      description: 'Vessel Name'    
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
      description: 'Date and time of this observation represented by an ISO 8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    owner:    
      description: 'A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)'    
      items:    
        anyOf:    
          - description: 'Property. Identifier format of any NGSI entity'    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
          - description: 'Property. Identifier format of any NGSI entity'    
            format: uri    
            type: string    
        description: 'Property. Unique identifier of the entity'    
      type: array    
      x-ngsi:    
        type: Property    
    ownerVessel:    
      description: 'Owner Vessel'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    photo:    
      description: 'Vessel Photo URL'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    previousPort:    
      description: 'Previous Port (Geographic coding scheme UN/LOCODE (United Nations Code for Trade and Transport Locations). https://unece.org/trade/publications/recommendation-ndeg16-united-nations-code-trade-and-transport-locations)'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    rateOfTurn:    
      description: 'Rate of Turn (ROT).'    
      maximum: 708    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' degree'    
    seeAlso:    
      description: 'list of uri pointing to additional resources about the item'    
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
    speedOverGround:    
      description: 'Speed Over Ground (SOG).'    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: ' meters per second'    
    technicalManager:    
      description: 'Technical Manager'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    toBow:    
      description: 'Dimension to Bow.'    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    toPort:    
      description: 'Dimension to Port.'    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    toStardboard:    
      description: 'Dimension to Starboard.'    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    toStern:    
      description: 'Dimension to Stern.'    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: ' meters'    
    type:    
      description: 'NGSI Entity type. It has to be Vessel'    
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
  x-model-schema: https://gitlab.com/hiades/fiware/smart-data-models/-/raw/main/dataModel.Vessel/schema.json    
  x-model-tags: ""    
  x-version: 0.0.1    
```  
</details>    
## Esempi di payload  
#### Vessel NGSI-v2 valori-chiave Esempio  
Ecco un esempio di un Vessel in formato JSON-LD come valori-chiave. Questo è compatibile con NGSI-v2 quando si usa `options=keyValues` e restituisce i dati di contesto di una singola entità.  
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
    "previousPort": "ESPMI"  
}  
```  
#### Vessel NGSI-v2 normalizzato Esempio  
Ecco un esempio di un Vessel in formato JSON-LD normalizzato. Questo è compatibile con NGSI-v2 quando non si utilizzano le opzioni e restituisce i dati di contesto di una singola entità.  
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
    }  
}  
```  
#### Valori chiave NGSI-LD del vaso Esempio  
Ecco un esempio di un Vessel in formato JSON-LD come valori-chiave. Questo è compatibile con NGSI-LD quando si usa `options=keyValues` e restituisce i dati di contesto di una singola entità.  
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
    "@context": [  
        "https://gitlab.com/hiades/fiware/smart-data-models/-/raw/main/context.jsonld"  
    ]  
}  
```  
#### Vaso NGSI-LD normalizzato Esempio  
Ecco un esempio di un Vessel in formato JSON-LD normalizzato. Questo è compatibile con NGSI-LD quando non si utilizzano le opzioni e restituisce i dati di contesto di una singola entità.  
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
    "@context": [  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.MarineTransport/master/context.jsonld"  
    ]  
}  
```  
Vedere [FAQ 10](https://smartdatamodels.org/index.php/faqs/) per ottenere una risposta su come gestire le unità di grandezza.  
