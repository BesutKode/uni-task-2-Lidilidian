#Pulau Pahawang

Pahawang island is one of most beautifull island in Indonesia, located in Lampung province, exactly in the district Pesawaran.

Tentang | Isi
---|---
Nama | Pulau Pahawang
Provinsi | [Lampung](https://id.wikipedia.org/wiki/Lampung)
Kota/Kabupaten | [Kabupaten Pesawaran](https://id.wikipedia.org/wiki/Kabupaten_Pesawaran)
Wikidata | [Q12506865](https://www.wikidata.org/wiki/Q12506865)
Wikipedia | [Pulau Pahawang](https://id.wikipedia.org/wiki/Pulau_Pahawang,_Punduh_Pidada,_Pesawaran)
Jumlah Populasi | 1.379 penduduk - [(sumber)](https://www.bps.go.id/website/fileMenu/Penduduk-Indonesia-Menurut-Desa-2010.pdf)
Area | 1.084 ha [(sumber)](http://www.cumilebay.com/2012/08/pulau-pahawang.html)
OSM Way id | [157314216](https://www.openstreetmap.org/way/157314216)
Koordinat | 5° 40' 26.65" S, 105° 13' 8.95" E
  | -5.674068, 105.219154 [WGS84 - GeoHack](https://tools.wmflabs.org/geohack/geohack.php?language=id&pagename=Pulau_Pahawang%2C_Punduh_Pidada%2C_Pesawaran&params=-5.6740676_N_105.2191544_E_)

For more info about Pahawang island see [pahawang_island_map.html^](https://htmlpreview.github.io/?https://raw.githubusercontent.com/BesutKode/uni-task-2-Lidilidian/master/pahawang_island_map.html?token=ARJl5Su-T_H81gHayKbHKseu6Aa0k_axks5YM2iCwA%3D%3D)


## How to get all data on this repository

### Perform query on [Overpass Turbo]http://overpass-turbo.eu/
Overpass turbo is a web based data mining tool for OpenStreetMap. It runs any kind of Overpass API query and shows the results on an interactive map. [source](http://wiki.openstreetmap.org/wiki/Overpass_turbo), to perform a search query data on Pahawang island, using OverpassQL which can be seen in [query.txt](https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/query.txt) and export the result to geojson for using it as layer data in [QGIS](http://www.qgis.org/en/site/).

### Edit the Map
Geojson.io is one of hundred of tools can manipulate the geojson file, for using it click [here](http://geojson.io), on Geojson.io click Open->File, select your geojson file, Geojson.io is divided into two parts where the left is a map view and the right side is a json file editor, for add some features like point, polyline, polygon, etc, You can simply use the existing tool on the map side. or if You want to manualy edit using JSON You can use JSON Editor in the right side, see [this](http://www.macwright.org/2015/03/23/geojson-second-bite.html#features) article for editing GeoJSON file. after finished add some features You can save it into various typedata, simply click Save->(choose your typedata)->select location to save. and done.

### Conver geojson to Image file
To convert the geojson file into image, use Your geojson data and add-it to QGIS, Open QGIS and choose Layers->Add Layer->Add Vector Layer, or simply do CTRL+SHIFT+V, and browse for the export file geojson from overpass-turbo, then, click Project->Save as Image and choose location to save the output (default output type is PNG)

### Convert geojson to shapefile* (* optional if need shapefile)
I do modifications [geoJSONToShpFile](https://github.com/TipsForGIS/geoJSONToShpFile) from TipsForGIS repo and make You can simply do the conversion from GeoJSON to shapefile, check [here](https://github.com/Lidilidian/geoJSONToShpFile)

##License

- This repository are using [MIT License]((https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/LICENSE.md))
- The data (kml, osm, qgs, topojson and geojson) are under [ODbL v1.0]((https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/LICENSE_ODbL.md))
- The source data about population in pahawang island is attributed to Badan Pusat Statistik (BPS) Indonesia under [CC-BY](https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/LICENSE_CC-BY.md) and the use of information based on : [UNDANG-UNDANG REPUBLIK INDONESIA NOMOR 14 TAHUN 2008](https://www.bps.go.id/website/fileMenu/fileMenu-15.pdf) , [PERATURAN PEMERINTAH REPUBLIK INDONESIA NOMOR 61 TAHUN 2010](https://www.bps.go.id/website/fileMenu/Peraturan-Pemerinrah-RI-No-61-Tahun-2010-tentang-Pelaksanaan-UU-No-14-Tahun-2008-tentang-KIP.pdf), and [PERATURAN KOMISI INFORMASI BADAN PUSAT STATISTIK REPUBLIK INDONESIA NOMOR 1 TAHUN 2010](https://www.bps.go.id/website/fileMenu/Peraturan-Komisi-Informasi-Nomor-1-Tahun-2010-tentang-Standar-Layanan-Informasi-Publik.pdf)
- All related artikel link to openstreetmap are under [CC BY-SA](http://creativecommons.org/licenses/by-sa/2.0/)
