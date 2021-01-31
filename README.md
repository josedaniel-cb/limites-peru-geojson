# Límites políticos de Perú en formato GeoJSON

Límites distritales, provinciales y departamentales de Perú en formato GeoJSON.

## Archivos

Versión detallada:

* [LIM_DISTRITAL_PERU.json](https://pip.pypa.io/)
* [LIM_PROVINCIAL_PERU.json](https://pip.pypa.io/)
* [LIM_DEPARTAMENTAL_PERU.json](https://pip.pypa.io/)

Versión simplificada:

* [LIM_DISTRITAL_PERU_MIN.json](https://pip.pypa.io/)
* [LIM_PROVINCIAL_PERU_MIN.json](https://pip.pypa.io/)
* [LIM_DEPARTAMENTAL_PERU_MIN.json](https://pip.pypa.io/)

## Contenido

+ Nivel distrital

```json
{
    "type": "Feature", 
    "geometry": {
        "type": "Polygon", 
        "coordinates": [
            [
                [-79.97797998918509, -5.026499972695547], 
                [-79.99197261374508, -5.024681598377015], 
                [-80.00224611356725, -5.015972597857058], 
                ...
            ]
        ]
    }, 
    "properties": {
        "CCDD": "20", 
        "NOMBDEP": "PIURA", 
        "CCPP": "04", 
        "NOMBPROV": "MORROPON", 
        "CCDI": "01", 
        "NOMBDIST": "CHULUCANAS", 
        "CAPITAL": "CHULUCANAS", 
        "UBIGEO": "200401", 
        "IDPROV": "2004", 
        "CODIGO": "200401", 
        "CNT_CCPP": 79, 
        "DESCRIPCIO": "CHULUCANAS"
    }
}
```

+ Nivel provincial

```json
{
    "type": "Feature", 
    "geometry": {
        "type": "Polygon", 
        "coordinates": [
            [
                [-79.64220898865386, -5.107216847679354], 
                [-79.65140623920655, -5.099867222794046], 
                [-79.6782599892071, -5.093549972852941],
                ...
            ]
        ]
    }, 
    "properties": {
        "OBJECTID_1": 64, 
        "OBJECTID": 61, 
        "CCDD": "20", 
        "NOMBDEP": "PIURA", 
        "CCPP": "04", 
        "NOMBPROV": "MORROPON", 
        "CAPITAL": "CHULUCANAS", 
        "IDPROV": "2004", 
        "Shape_STAr": 0.308883712248, 
        "Shape_STLe": 3.44473263743, 
        "ORIG_FID": 60, 
        "Shape_Leng": 3.44473264274, 
        "Shape_Area": 0.308883712253
    }
}
```

+ Nivel departamental

```json
{
    "type": "Feature", 
    "geometry": {
        "type": "Polygon", 
        "coordinates": [
            [
                [-80.4873319886803, -4.083128846818795], 
                [-80.51093949006537, -4.093576221565343], 
                [-80.52434573956418, -4.107414097082881], 
                ...
            ]
        ]
    }, 
    "properties": {
        "OBJECTID_1": 23, 
        "OBJECTID": 20, 
        "CCDD": "20", 
        "NOMBDEP": "PIURA", 
        "CAPITAL": "PIURA", 
        "Shape_STAr": 2.89922289074, 
        "Shape_STLe": 11.2994707345, 
        "ORIG_FID": 19, 
        "Shape_Leng": 11.2994707354, 
        "Shape_Area": 2.89922289077
    }
}
```

## Elaboración
Los archivos en formato Shapefile fueron convertidos a GeoJSON haciendo uso de Mapshaper y simplificados mediante el método Visvalingam al 5%.

## Fuentes de datos

[geogpsperu.com](https://www.geogpsperu.com/)
+ [Limite Distrital](https://www.geogpsperu.com/2019/05/limite-distrital-actualizado-inei.html)
+ [Limite Provincial](https://www.geogpsperu.com/2019/08/limite-provincial-politico-shapefile.html)
+ [Limite Departamental](https://www.geogpsperu.com/2019/08/limite-departamental-politico-shapefile.html)

## Recursos
+ [mapshaper](https://mapshaper.org/)

## Enlaces de interés
+ [Convert ESRI Shapefile Map to GeoJSON format](https://www.statsilk.com/maps/convert-esri-shapefile-map-geojson-format)

## License
[MIT](https://choosealicense.com/licenses/mit/)