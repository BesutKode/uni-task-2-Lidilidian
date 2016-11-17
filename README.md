# PAHAWANG ISLAND

Pahawang island is one of most beautifull island in Indonesia, located in Lampung province, exactly in the Pesawaran regency.

About | Detail
---|---
Name | Pulau Pahawang
Province | [Lampung](https://id.wikipedia.org/wiki/Lampung)
City/Regency | [Kabupaten Pesawaran](https://id.wikipedia.org/wiki/Kabupaten_Pesawaran)
Wikidata | [Q12506865](https://www.wikidata.org/wiki/Q12506865)
Wikipedia | [Pulau Pahawang](https://id.wikipedia.org/wiki/Pulau_Pahawang,_Punduh_Pidada,_Pesawaran)
Population | 1.379 people - [(source)](https://www.bps.go.id/website/fileMenu/Penduduk-Indonesia-Menurut-Desa-2010.pdf)
Area | 1.084 ha [(source)](http://www.cumilebay.com/2012/08/pulau-pahawang.html)
OSM Way id | [157314216](https://www.openstreetmap.org/way/157314216)
Postal Code | 35453 [(source)](http://nomorkodepos.com/di/lampung/pesawaran/marga-punduh/pulau-pahawang/)
Coordinate | 5° 40' 26.65" S, 105° 13' 8.95" E
  | -5.674068, 105.219154 [WGS84 - GeoHack](https://tools.wmflabs.org/geohack/geohack.php?language=id&pagename=Pulau_Pahawang%2C_Punduh_Pidada%2C_Pesawaran&params=-5.6740676_N_105.2191544_E_)
Maps | [Pahawang Island](https://besutkode.github.io/uni-task-2-Lidilidian/)

For more info about Pahawang island see :
- [Pahawang Island](https://besutkode.github.io/uni-task-2-Lidilidian/) Maps
- http://www.utiket.com/id/obyek-wisata/bandar_lampung/423-menikmati_pulau_pahawang.html


# How to get all data on this repository

## Raw GeoJSON of Pahawang island 

### Perform query on [Overpass Turbo](http://overpass-turbo.eu/)
Overpass turbo is a web based data mining tool for OpenStreetMap. It runs any kind of Overpass API query and shows the results on an interactive map. [source](http://wiki.openstreetmap.org/wiki/Overpass_turbo), to perform a search query data on Pahawang island, using OverpassQL which can be seen in [query.txt](https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/query.txt) and export the result to geojson for using it as layer data in [QGIS](http://www.qgis.org/en/site/).


## Data Information about Pahawang Island

### Data Batas Administrasi
The Data about `Data Batas Administrasi` can be download in [Portal Data Indonesia](http://portal.ina-sdi.or.id/arcgis/rest/services/IGD/RupabumiIndonesia/MapServer) i also create a mirro [here](https://drive.google.com/file/d/0B2k9p5nUCGRvTUg4ZkJRX1A5dVk/view?usp=sharing) since November 17th, 2016 till idk, the MapServer is under maintenance, i'm sorry can't upload/mirror-it on github due my internet connection was unstable.

### Daerah Aliran Sungai
The Data about `Daerah Aliran Sungai` can be download in [APPGIS Dephut Indonesia](http://appgis.dephut.go.id/appgis/download.aspx), choose the area You wan to download the data, in this repo i use [Sumatera.kml](http://appgis.dephut.go.id/appgis/download.aspx?status=view&filename=Sulawesi.kml&fileFullName=E:\webgis1\Peta%20Tematik%20Kehutanan1\KML\Daerah%20Aliran%20Sungai\Sulawesi.kml), note : the data format is KML not geojson to convert it yout can use this [2geojson.com](http://2geojson.com/)

## Editing the Map
Convert all data where file type isn't geojson to geojson using QGIS, Open QGIS, for importing vector layer like geojson, kml and shapefile (and more) simply do CTRL+SHIFT+V (i do this on my Laptop using GNU/Linux [OpenSUSE Leap](https://software.opensuse.org/422/en) choose file (for single file like geojson/kml) or directory (shapefile) then locate your file that you download before, after load all data then click Project->DXF Export, choose you location to save export file, chang symbol to 'feature symbology' then ok, now you have DXF file with all data layer merge.

next, convert DXF to geojson, open [2geojson.com](http://2geojson.com/), select format 'DXF', locate your DXF file, leave other to default then click submit, now you have all data layer merge in geojson. for editing the geojson use geojson.io.

Geojson.io is one of hundred of tools can manipulate the geojson file, for using it click [here](http://geojson.io), on Geojson.io click Open->File, select your geojson file, Geojson.io is divided into two parts where the left is a map view and the right side is a json file editor, for add some features like point, polyline, polygon, etc, You can simply use the existing tool on the map side. or if You want to manualy edit using JSON You can use JSON Editor in the right side, see [this](http://www.macwright.org/2015/03/23/geojson-second-bite.html#features) article for editing GeoJSON file. after finished add some features You can save it into various typedata, simply click Save->(choose your typedata)->select location to save. and done.

### Convert geojson to Image file
To convert the geojson file into image, use Your geojson data and add-it to QGIS, Open QGIS and choose Layers->Add Layer->Add Vector Layer, or simply do CTRL+SHIFT+V, and browse for the export file geojson from overpass-turbo, then, click Project->Save as Image and choose location to save the output (default output type is PNG)

### Convert geojson to shapefile* (* optional if need shapefile)
I do modifications [geoJSONToShpFile](https://github.com/TipsForGIS/geoJSONToShpFile) from TipsForGIS repo and make You can simply do the conversion from GeoJSON to shapefile, check [here](https://github.com/Lidilidian/geoJSONToShpFile)

##License

- This repository are using [MIT License](https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/LICENSE)
- Data `kml, osm, qgs, topojson and geojson` are under [ODbL v1.0](https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/license/LICENCSE_ODbL.md)
- Data about `Batas Administrasi` and `Daerah Aliran Sungai` are under [CC-BY](http://www.opendefinition.org/licenses/cc-by) , based on [Portal Data Indonesia](http://www.data.go.id)
- The source data about `population` in pahawang island is attributed to `Badan Pusat Statistik (BPS)` Indonesia under [CC-BY](https://github.com/BesutKode/uni-task-2-Lidilidian/blob/master/LICENSE_CC-BY.md) and the use of information based on : [UNDANG-UNDANG REPUBLIK INDONESIA NOMOR 14 TAHUN 2008](https://www.bps.go.id/website/fileMenu/fileMenu-15.pdf) , [PERATURAN PEMERINTAH REPUBLIK INDONESIA NOMOR 61 TAHUN 2010](https://www.bps.go.id/website/fileMenu/Peraturan-Pemerinrah-RI-No-61-Tahun-2010-tentang-Pelaksanaan-UU-No-14-Tahun-2008-tentang-KIP.pdf), and [PERATURAN KOMISI INFORMASI BADAN PUSAT STATISTIK REPUBLIK INDONESIA NOMOR 1 TAHUN 2010](https://www.bps.go.id/website/fileMenu/Peraturan-Komisi-Informasi-Nomor-1-Tahun-2010-tentang-Standar-Layanan-Informasi-Publik.pdf)
- All related artikel link to openstreetmap are under [CC BY-SA](http://creativecommons.org/licenses/by-sa/2.0/)
