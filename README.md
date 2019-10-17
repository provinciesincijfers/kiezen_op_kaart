# kiezen op kaart in Swing Jive

Een tooltje om het mogelijk te maken één of meerdere gebieden te selecteren op basis van een kaart.

Ingebouwd op [provincies.incijfers.be](https://provincies.incijfers.be/databank?report=kiezen_op_kaart&keepworkspace=true). Mag  hergebruikt worden in andere Swing-versies of als stand-alone mits verwijzing naar deze pagina.

Ontwikkeld door [@jbelien](https://github.com/jbelien) via [Geo-6](https://geo-6.be/).

## Gebiedsniveaus toevoegen/aanpassen

* gebieden
- open je geometrie in QGIS
- hou enkel de unieke code en de naam. Gebruik hiervoor veldnamen "geoitem" en "naam".
- sla op als geojson in WGS84 (epsg 4326). Precisie van de coordinaten eventueel van 15 naar 6. 
- vereenvoudig de geometrie; file-size liefst zo veel mogelijk onder de 5 mb. http://mapshaper.org/ is hier heel handig voor. De output daar is een .json bestand, maar eigenlijk is dit GeoJSON. Maakt niet uit, en wij veranderen de extentie toch naar .txt om het handig bewerkbaar binnen Swing te maken.
- wij bewaren de bestanden in de map https://provincies.incijfers.be/Report/GeoJSON/ met namen als "gemeente4326_simp.txt". Opgeelt: de code verwijst naar de -gepubliceerde- versie. Als je aan het testen bent, moet je dus nog /admin toevoegen aan de URL van de bestanden.
