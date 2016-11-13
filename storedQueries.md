# Stored queries


## GetDataSetById
__GetDataSetById__

    GetDataSetById returns INSPIRE data sets. Consult catalog.fmi.fi to investigate possible data sets.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| datasetid | xsi:string | Data set ID |  |





## Aviation weather from aerodromes in Finland
__fmi::avi::observations::finland::iwxxm__

    This stored query return aviation weather messages from the essential aerodromes in Finland (predefined aerodrome set). Each message is constructed from a METAR weather report and converted to IWXXM (ICAO Meteorological Information Exchange Model) format. By default, the data is returned from the last 60 minutes. One can change the time range by using starttime and endtime parameters. It is also possible to request additional aerodromes which are included into the predefined aerodrome set by using icaocode parameter (duplicates are iqnored).
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of time interval |  
 endtime | xsi:dateTime | End of time interval |  
 icaocode | xsi:string | ICAO Code |  |





## Aviation weather from aerodromes in Finland
__fmi::avi::observations::finland::latest::iwxxm__

    This stored query return the latest aviation weather messages (one per aerodrome) from the essential aerodromes in Finland (predefined aerodrome set). Each message is constructed from a METAR weather report and converted to IWXXM (ICAO Meteorological Information Exchange Model) format. By default, the latest messages are searched from the last 24 hours. One can change the time range by using starttime and endtime parameters. It is also possible to request additional aerodromes which are included into the predefined aerodrome set by using icaocode parameter (duplicates are ignored).
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of time interval |  
 endtime | xsi:dateTime | End of time interval |  
 icaocode | xsi:string | ICAO Code |  |





## Aviation weather from aerodromes
__fmi::avi::observations::iwxxm__

    This stored query return aviation weather messages. Each message is constructed from a METAR weather report and converted to IWXXM (ICAO Meteorological Information Exchange Model) format. By default, the data is returned from the 60 minutes. One can change the time range by using starttime and endtime parameters. At least one location parameter (icaocode, bbox, geoid) must be given to get non zero result.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 icaocode | xsi:string | ICAO Code |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 geoid | int | Geoid of the location for which to return data. |  |





## Aviation weather from aerodromes
__fmi::avi::observations::latest::iwxxm__

    This stored query return the latest aviation weather messages from aerodromes. Each message is constructed from a METAR weather report and converted to IWXXM (ICAO Meteorological Information Exchange Model) format. By default, the latest message is searched from the last 24 hours. One can change the time range by using starttime and endtime parameters. At least one location parameter (icaocode, bbox, geoid) must be given to get non zero result.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 icaocode | xsi:string | ICAO Code |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 geoid | int | Geoid of the location for which to return data. |  |





## Climate Scenarios
__fmi::forecast::climatology::scenario::grid__

    Mean temperature and precipitation amount scenarios for three periods of thirty years. The data contains 10x10km grid and is returned in GRIB format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 parameters | NameList | Parameters to return |  |





## HBM Current Model Grid
__fmi::forecast::hbm::grid__

    HBM forecast model provides sea currents and water temperature forecast as grid data encoded in GRIB format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 parameters | NameList | Parameters to return |  
 format | xsi:string | Dataset format. |  
 levels | gml:integerList | Vertical level |  |





## HBM Current Model Point
__fmi::forecast::hbm::point::multipointcoverage__

    HBM forecast model provides sea currents and water temperature forecast. This stored query provides the data as point data encoded in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 latlon | gml:pos | Location coordinates to return data. |  
 geoid | int | Geoid of the location for which to return data. |  |





## HBM Current Model Point
__fmi::forecast::hbm::point::simple__

    HBM forecast model provides sea currents and water temperature forecast. This stored query provides the data as point data encoded in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 latlon | gml:pos | Location coordinates to return data. |  
 geoid | int | Geoid of the location for which to return data. |  |





## HBM Current Model Point
__fmi::forecast::hbm::point::timevaluepair__

    HBM forecast model provides sea currents and water temperature forecast. This stored query provides the data as point data encoded in time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 timestep | int | The time step of data in minutes |  
 latlon | gml:pos | Location coordinates to return data. |  
 geoid | int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Helsinki multi-category ice model as a grid.
__fmi::forecast::helmi::grid__

    This Stored Query request retrieve Helsinki multi-category ice model forecast raw dataset as a grid.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| producer | xsi:string | Producer |  
 starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 format | xsi:string | Dataset format. |  |





## Hirlam Pressure Grid
__fmi::forecast::hirlam::pressure::grid__

    Hirlam forecast model's pressure levels as a grid data encoded in GRIB format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 parameters | NameList | Parameters to return |  
 levels | gml:integerList | Pressure levels |  
 format | xsi:string | Dataset format. |  |





## Hirlam weather forecast for cities in Finland as multipointcoverage
__fmi::forecast::hirlam::surface::cities::multipointcoverage__

    This stored query fetch Hirlam weather forecast for cities in Finland. The forcast is returned in multi point coverage format. By default, forcast is returned for the next 36 hours.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Hirlam weather forecast for cities in Finland as simple features
__fmi::forecast::hirlam::surface::cities::simple__

    This stored query fetch Hirlam weather forecast for cities in Finland. The forcast is returned in simple feature format. By default, forcast is returned for the next 36 hours.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Hirlam weather forecast for cities in Finland as time value pairs
__fmi::forecast::hirlam::surface::cities::timevaluepair__

    This stored query fetch Hirlam weather forecast for cities in Finland. The forcast is returned as time value pairs. By default, forcast is returned for the next 36 hours.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 timestep | int | The time step of data in minutes |  
 timezone | xsi:string | Time zone |  |





## Hirlam surface level weather forecast for Finland as a grid.
__fmi::forecast::hirlam::surface::finland::grid__

    This Stored Query request retrieve Hirlam surface level forecast raw dataset as a grid for Finland region.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| producer | xsi:string | Producer |  
 starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 format | xsi:string | Dataset format. |  |





## Hirlam Surface Grid
__fmi::forecast::hirlam::surface::grid__

    Hirlam forecast model's surface level as grid data encoded in GRIB format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 parameters | NameList | Parameters to return |  
 format | xsi:string | Dataset format. |  |





## Hirlam weather forecast for observation stations as multipointcoverage.
__fmi::forecast::hirlam::surface::obsstations::multipointcoverage__

    This stored query fetch Hirlam weather forecast for observation stations in Finland. The forcast is returned as multipointcoverage form. By default, forecast is returned for the next 36 hours.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 timestep | int | The time step of data in minutes |  |





## Hirlam weather forecast for observation stations as simple feature.
__fmi::forecast::hirlam::surface::obsstations::simple__

    This stored query fetch Hirlam weather forecast for observation stations in Finland. The forcast is returned as simple feature form. By default, forecast is returned for the next 36 hours.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 timestep | int | The time step of data in minutes |  |





## Hirlam weather forecast for observation stations as time value pairs.
__fmi::forecast::hirlam::surface::obsstations::timevaluepair__

    This stored query fetch Hirlam weather forecast for observation stations in Finland. The forcast is returned as time value pairs. By default, forecast is returned for the next 36 hours.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 timestep | int | The time step of data in minutes |  
 timezone | xsi:string | Time zone |  |





## Hirlam Point Weather Forecast as multipointcoverage
__fmi::forecast::hirlam::surface::point::multipointcoverage__

    Hirlam weather forecast fetched to a specific location returned in multi point coverage format. Location need to be specified as place or geoid or latlon query parameters.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 place | xsi:string | The location for which to provide data |  
 latlon | gml:pos | Location coordinates to return data. |  
 geoid | int | Geoid of the location for which to return data. |  |





## Hirlam Point Weather Forecast as simple features
__fmi::forecast::hirlam::surface::point::simple__

    Hirlam weather forecast fetched to a specific location returned in simple feature format. Location need to be specified as place or geoid or latlon query parameters.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 place | xsi:string | The location for which to provide data |  
 latlon | gml:pos | Location coordinates to return data. |  
 geoid | int | Geoid of the location for which to return data. |  |





## Hirlam Point Weather Forecast as time value pairs
__fmi::forecast::hirlam::surface::point::timevaluepair__

    Hirlam weather forecast fetched to a specific location returned in time value pair format. Location need to be specified as place or geoid or latlon query parameters.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 place | xsi:string | The location for which to provide data |  
 latlon | gml:pos | Location coordinates to return data. |  
 geoid | int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## OAAS Sea Level Model Point
__fmi::forecast::oaas::sealevel::point::multipointcoverage__

    OAAS forecast model provides sea level height forecast to points. This stored query provides point data encoded in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 crs | xsi:string | Coordinate projection to use in results |  
 geoid | int | Geoid of the location for which to return data. |  
 latlon | gml:pos | Location coordinates to return data. |  |





## OAAS Sea Level Model Point
__fmi::forecast::oaas::sealevel::point::simple__

    OAAS forecast model provides sea level height forecast to points. This stored query provides point data encoded in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 crs | xsi:string | Coordinate projection to use in results |  
 latlon | gml:pos | Location coordinates to return data. |  
 geoid | int | Geoid of the location for which to return data. |  |





## OAAS Sea Level Model Point
__fmi::forecast::oaas::sealevel::point::timevaluepair__

    OAAS forecast model provides sea level height forecast to points. This stored query provides point data encoded in time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 crs | xsi:string | Coordinate projection to use in results |  
 geoid | int | Geoid of the location for which to return data. |  
 latlon | gml:pos | Location coordinates to return data. |  
 timezone | xsi:string | Time zone |  |





## WAM Wave Model Grid
__fmi::forecast::wam::grid__

    WAM forecast model provides wave height forecast as grid data encoded in GRIB format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 parameters | NameList | Parameters to return |  |





## WAM Wave Model Point
__fmi::forecast::wam::point::multipointcoverage__

    WAM forecast model provides wave height forecast. This stored query provides point data encoded in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 geoid | int | Geoid of the location for which to return data. |  
 latlon | gml:point | Location coordinates to return data. |  |





## WAM Wave Model Point
__fmi::forecast::wam::point::simple__

    WAM forecast model provides wave height forecast. This stored query provides point data encoded in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 geoid | int | Geoid of the location for which to return data. |  
 latlon | gml:point | Location coordinates to return data. |  |





## WAM Wave Model Point
__fmi::forecast::wam::point::timevaluepair__

    WAM forecast model provides wave height forecast. This stored query provides point data encoded in time value pair format. Location has to be specified as geoid or latlon-coordinates.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 geoid | int | Geoid of the location for which to return data. |  
 latlon | gml:pos | Location coordinates to return data. |  
 timezone | xsi:string | Time zone |  |





## Hourly Air Quality Observations
__fmi::observations::airquality::hourly::multipointcoverage__

    Hourly air quality observations from weather stations of Finnish Meteorological Institute. By default, all the station are selected and the data is returned from the last 24 hours. The data is returned as multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  |





## Hourly Air Quality Observations
__fmi::observations::airquality::hourly::simple__

    Hourly air quality observations from weather stations or Finnish Meteorological Institute. By default, all the station are selected and the data is returned from the last 24 hours. The data is returned as a simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Hourly Air Quality Observations
__fmi::observations::airquality::hourly::timevaluepair__

    Hourly air quality observations from weather stations of Finnish Meteorological Institute. By default, all the station are selected and the data is returned from the last 24 hours. The data is returned as timevaluepair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Lightning Strikes
__fmi::observations::lightning::multipointcoverage__

    The response contains all detected lightning strikes in Finland. Observations are mainly ground flashes but some of cloud flashes are also detected.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  |





## Lightning Strikes
__fmi::observations::lightning::simple__

    The response contains all detected lightning strikes in Finland. Observations are mainly ground flashes but some of cloud flashes are also detected.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  |





## Mareograph Observations
__fmi::observations::mareograph::multipointcoverage__

    Water level observations from 13 locations. Time step is 60 minutes. The data is retuned in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  |





## Mareograph Observations
__fmi::observations::mareograph::simple__

    Water level observations from 13 locations. Time step is 60 minutes. The data is retuned in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  |





## Mareograph Observations
__fmi::observations::mareograph::timevaluepair__

    Water level observations from 13 locations. Time step is 60 minutes. The data is returned in time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  
 timezone | xsi:string | Time zone |  |





## Sun Radiation Observations
__fmi::observations::radiation::multipointcoverage__

    Sun radiation observations from weather stations. By default the data is returned from last 1 hour and from stations in Sodankylä, Jokioinen, Helsinki, Parainen, Vantaa, Jyväskylä, Sotkamo and Utsjoki. The data is returned in 'multipointcoverage' format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  |





## Sun Radiation Observations
__fmi::observations::radiation::simple__

    Sun radiation observations from weather stations. By default the data is returned from last 1 hour and from stations in Sodankylä, Jokioinen, Helsinki, Parainen, Vantaa, Jyväskylä, Sotkamo and Utsjoki. The data is returned in 'simple feature' format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  |





## Sun Radiation Observations
__fmi::observations::radiation::timevaluepair__

    Sun radiation observations from weather stations. By default the data is returned from last 1 hour and from stations in Sodankylä, Jokioinen, Helsinki, Parainen, Vantaa, Jyväskylä, Sotkamo and Utsjoki. The data is returned in 'timevaluepair' format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 maxlocations | int | Amount of locations |  
 fmisid | int | FMI observation station identifier. |  
 timezone | xsi:string | Time zone |  |





## Hourly Soil Observations
__fmi::observations::soil::hourly::multipointcoverage__

    Hourly minimum, maximum and average soil values from weather stations. By default, the data is returned from last 12 hour.  At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned as multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Hourly Soil Observations
__fmi::observations::soil::hourly::simple__

    Hourly minimum, maximum and average soil values from weather stations. By default, the data is returned from last 12 hour.  At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned as simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Hourly Soil Observations
__fmi::observations::soil::hourly::timevaluepair__

    Hourly minimum, maximum and average soil values from weather stations. By default, the data is returned from last 12 hour.  At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned as a time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Wave and Water temperature observations
__fmi::observations::wave::multipointcoverage__

    Wave and water temperature observations from buoys. Available parameters are significant wave height, wave direction, deviation of wave direction, modal period and water temperature. Some buoys return only temperature values. Time step is 30 minutes. The data is returned in multipointcoverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  |





## Wave and Water temperature observations
__fmi::observations::wave::simple__

    Wave and water temperature observations from buoys. Available parameters are significant wave height, wave direction, deviation of wave direction, modal period and water temperature. Some buoys return only temperature values. Time step is 30 minutes. The data is returned in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  |





## Wave and Water temperature observations
__fmi::observations::wave::timevaluepair__

    Wave and water temperature observations from buoys. Available parameters are significant wave height, wave direction, deviation of wave direction, modal period and water temperature. Some buoys return only temperature values. Time step is 30 minutes. The data is returned in time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 fmisid | int | FMI observation station identifier. |  
 timezone | xsi:string | Time zone |  |





## Weather observations for cities as multipointcoverage.
__fmi::observations::weather::cities::multipointcoverage__

    Weather observations for cities in Finland as multipointcoverage.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 timestep | xsi:unsignedInteger | The time step in minutes |  |





## Weather observations for cities as simple feature.
__fmi::observations::weather::cities::simple__

    Weather observations for cities in Finland as simple feature.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 timestep | xsi:unsignedInteger | The time step in minutes |  |





## Weather observations for cities as time value pairs.
__fmi::observations::weather::cities::timevaluepair__

    Weather observations for cities in Finland as time value pairs.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 timestep | xsi:unsignedInteger | The time step of data in minutes |  
 timezone | xsi:string | Time zone |  |





## Daily Weather Observations
__fmi::observations::weather::daily::multipointcoverage__

    Daily weather observations from weather stations. Default set contains daily precipitation rate, mean temperature, snow depth, and minimum  and maximum temperature. By default, the data is returned from last 744 hours. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  |





## Daily Weather Observations
__fmi::observations::weather::daily::simple__

    Daily weather observations from weather stations. Default set contains daily precipitation rate, mean temperature, snow depth, and minimum  and maximum temperature. By default, the data is returned from last 744 hours. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  |





## Daily Weather Observations
__fmi::observations::weather::daily::timevaluepair__

    Daily weather observations from weather stations. Default set contains daily precipitation rate, mean temperature, snow depth, minimum temperature and maximum temperature. By default, the data is returned from last 744 hours. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Instantaneous profile observations from masts
__fmi::observations::weather::mast::multipointcoverage__

    This stored query return instantaneous profile observations from masts in multipointcoverage format. By default latest observation of the available meteo paramters are returned in 10 minute resolution. At least one location has to be given.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  |





## Monthly weather observations of 30-year normal period
__fmi::observations::weather::monthly::30year::multipointcoverage__

    Monthly Weather Observations of 30-year normal period. By default, the data is returned from the normal period of 1981 - 2010. There is available the following normal periods: 1971 - 2000, 1981 - 2010. Notice that there is only data at the begin of the period. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Monthly weather observations of 30-year normal period
__fmi::observations::weather::monthly::30year::simple__

    Monthly Weather Observations of 30-year normal period. By default, the data is returned from the normal period of 1981 - 2010. There is available the following normal periods: 1971 - 2000, 1981 - 2010. Notice that there is only data at the begin of the period. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Monthly weather observations of 30-year normal period
__fmi::observations::weather::monthly::30year::timevaluepair__

    Monthly Weather Observations of 30-year normal period. By default, the data is returned from the normal period of 1981 - 2010. There is available the following normal periods: 1971 - 2000, 1981 - 2010. Notice that there is only data at the begin of the period. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Monthly Weather Observations
__fmi::observations::weather::monthly::grid__

    Monthly precipitation rate and mean temperature interpolated into a grid. The data is returned in GRIB format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 parameters | NameList | Parameters to return |  |





## Monthly Weather Observations
__fmi::observations::weather::monthly::multipointcoverage__

    Monthly weather observations from weather stations. Default set contains monthly precipitation rate, mean temperature. By default, the data is returned from last 12 months. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  |





## Monthly Weather Observations
__fmi::observations::weather::monthly::simple__

    Monthly weather observations from weather stations. Default set contains monthly precipitation rate, mean temperature. By default, the data is returned from last 12 months. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  |





## Monthly Weather Observations
__fmi::observations::weather::monthly::timevaluepair__

    Monthly weather observations from weather stations. Default set contains monthly precipitation rate, mean temperature. By default, the data is returned from last 12 months. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Instantaneous Weather Observations
__fmi::observations::weather::multipointcoverage__

    Real time weather observations from weather stations. Default set contains wind speed, direction, gust, temperature, relative humidity, dew point, pressure reduced to sea level, one hour precipitation amount, visibility and cloud cover. By default, the data is returned from last 12 hour. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned as a multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  |





## Instantaneous Weather Observations
__fmi::observations::weather::simple__

    Real time weather observations from weather stations. Default set contains wind speed, direction, gust, temperature, relative humidity, dew point, pressure reduced to sea level, one hour precipitation amount, visibility and cloud cover. By default, the data is returned from last 12 hour. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned as a simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  |





## Instantaneous Weather Observations
__fmi::observations::weather::timevaluepair__

    Real time weather observations from weather stations. Default set contains air temperatire, wind speed, gust speed, wind direction, relative humidity, dew point, one hour precipitation amount, precipitation intensity, snow depth, pressure reduced to sea level and visibility. By default, the data is returned from last 12 hour.  At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned as a time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Yearly weather observations of 30-year normal period
__fmi::observations::weather::yearly::30year::multipointcoverage__

    Yearly Weather Observations of 30-year normal period. By default, the data is returned from the normal period of 1981 - 2010. There is available the following normal periods: 1971 - 2000, 1981 - 2010. Notice that there is only data at the begin of the period. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Yearly weather observations of 30-year normal period
__fmi::observations::weather::yearly::30year::simple__

    Yearly Weather Observations of 30-year normal period. By default, the data is returned from the normal period of 1981 - 2010. There is available the following normal periods: 1971 - 2000, 1981 - 2010. Notice that there is only data at the begin of the period. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Yearly weather observations of 30-year normal period
__fmi::observations::weather::yearly::30year::timevaluepair__

    Yearly Weather Observations of 30-year normal period. By default, the data is returned from the normal period of 1981 - 2010. There is available the following normal periods: 1971 - 2000, 1981 - 2010. Notice that there is only data at the begin of the period. At least one location parameter (geoid/place/fmisid/wmo/bbox) has to be given. The data is returned in time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 wmo | int | WMO code of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Radar
__fmi::radar__

    All available radar images during last hour.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Radar Reflectivity Composite
__fmi::radar::composite::dbz__

    Radar reflectivity (dbz) as composite covering Finland.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Precipitation Rate Composite
__fmi::radar::composite::rr__

    Precipitation rate (rr) as composite covering Finland.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Precipitation Amount 12h Composite
__fmi::radar::composite::rr12h__

    Precipitation amount of twelve hours (rr12h) as composite covering Finland.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Precipitation Amount 1h Composite
__fmi::radar::composite::rr1h__

    Precipitation amount of one hour (rr1h) as composite covering Finland.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Precipitation Amount 24h Composite
__fmi::radar::composite::rr24h__

    Precipitation amount of 24 hours (rr24h) as composite covering Finland.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Radar Reflectivity Single
__fmi::radar::single::dbz__

    Radar reflectivity (dbz) from single radars.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 elevation | string | Elevation |  |





## Echo Top Single
__fmi::radar::single::etop_20__

    Echo top 20 (etop_20) from single radars.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Hydro Class Single
__fmi::radar::single::hclass__

    Hydro class (hclass) from single radars.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Doppler Speed Single
__fmi::radar::single::vrad__

    Doppler speed (vrad) from single radars.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Surface level Hilatar model deposition data
__fmi::transportmodel::hilatar::surface::scandinavia::grid__

    This Stored Query retrieve simulated surface level deposition of nitrogen and sulphur compounds in Scandinavia in units mg per m2 (S or N) in the selected time period. Data is available in NetCDF file format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 parameters | gml:NameList | Parameters to return |  
 bbox | xsi:string | Bounding box of area for which to return data. |  |





## Instantaneous Road Weather Observations
__livi::observations::road::default::multipointcoverage__

    Real time road weather observations from road weather stations. By default, basic weather data is returned from last 20 minutes. At least one location parameter (geoid/place/fmisid/bbox) has to be given. The data is returned as a multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | xsi:int | FMI observation station identifier. |  
 maxlocations | xsi:int | Amount of locations |  
 geoid | xsi:int | Geoid of the location for which to return data. |  |





## Instantaneous Road Weather Observations
__livi::observations::road::default::simple__

    Real time road weather observations from road weather stations. By default, basic weather data is returned from last 20 minutes. At least one location parameter (geoid/place/fmisid/bbox) has to be given. The data is returned as a simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | xsi:int | FMI observation station identifier. |  
 maxlocations | xsi:int | Amount of locations |  
 geoid | xsi:int | Geoid of the location for which to return data. |  |





## Instantaneous Road Weather Observations
__livi::observations::road::default::timevaluepair__

    Real time road weather observations from road weather stations. By default, essential parameters are returned from last 20 minutes. At least one location parameter (geoid/place/fmisid/bbox) has to be given. The data is returned as a time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | xsi:int | FMI observation station identifier. |  
 maxlocations | xsi:int | Amount of locations |  
 geoid | xsi:int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Instantaneous Road Weather Observations
__livi::observations::road::finland::multipointcoverage__

    Real time road weather observations from road weather stations in Finland. By default, essential parameters are returned from last 20 minutes. The data is returned as a multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  |





## Instantaneous Road Weather Observations
__livi::observations::road::finland::simple__

    Real time road weather observations from road weather stations in Finland. By default, essential parameters are returned from last 20 minutes. The data is returned as a simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  |





## Instantaneous Road Weather Observations
__livi::observations::road::finland::timevaluepair__

    Real time road weather observations from road weather stations in Finland. By default, essential parameters are returned from last 20 minutes. The data is returned as a time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  
 timezone | xsi:string | Time zone |  |





## Instantaneous Road Weather Observations
__livi::observations::road::multipointcoverage__

    Real time road weather observations from road weather stations. By default, the data is returned from last 12 hours. At least one location parameter (geoid/place/fmisid/bbox) has to be given. The data is returned as a multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | xsi:int | FMI observation station identifier. |  
 maxlocations | xsi:int | Amount of locations |  
 geoid | xsi:int | Geoid of the location for which to return data. |  |





## Instantaneous Road Weather Observations
__livi::observations::road::simple__

    Real time road weather observations from road weather stations. By default, the data is returned from last 12 hours. At least one location parameter (geoid/place/fmisid/bbox) has to be given. The data is returned as a simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | xsi:int | FMI observation station identifier. |  
 maxlocations | xsi:int | Amount of locations |  
 geoid | xsi:int | Geoid of the location for which to return data. |  |





## Instantaneous Road Weather Observations
__livi::observations::road::timevaluepair__

    Real time road weather observations from road weather stations. By default, the data is returned from last 12 hours. At least one location parameter (geoid/place/fmisid/bbox) has to be given. The data is returned as a time value pair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | xsi:dateTime | Begin of the time interval |  
 endtime | xsi:dateTime | End of time interval |  
 timestep | xsi:int | The time step of data in minutes |  
 parameters | gml:NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | xsi:int | FMI observation station identifier. |  
 maxlocations | xsi:int | Amount of locations |  
 geoid | xsi:int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Radioactivity in outdoor air
__stuk::observations::air::radionuclide-activity-concentration::latest::multipointcoverage__

    This stored query returns only the latest results of the measurement of the radioactivity samples collected by special equipment. At monitoring station samples are created by pumping high volumes of air through glass fibre filter. In Finland there are 8 monitoring stations. By default all the monitoring stations are selected and the latest results of measurements are search from the last 720 hours. The default values can be overwritten by using the time and location related input parameters.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 geoid | int | Geoid of the location for which to return data. |  
 maxlocations | int | Amount of locations |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Radioactivity in outdoor air
__stuk::observations::air::radionuclide-activity-concentration::latest::simple__

    This stored query return only the latest results of measurement of radioactivity samples collected by special equipment that filtering outdoor air in the monitoring stations in Finland. By default all the monitoring stations are selected and the latest results of measurements are search from the last 720 hours. The default values can be overwritten by using the time and location related input parameters. Notice that a result member contains the coordinates of a monitoring station, the endtime of sample collection period, a nuclide code and measured activity concentration.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 nuclides | NameList | Radionuclides to return |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 geoid | int | Geoid of the location for which to return data. |  
 maxlocations | int | Amount of locations |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Radioactivity in outdoor air
__stuk::observations::air::radionuclide-activity-concentration::multipointcoverage__

    This stored query returns the results of the measurement of the radioactivity samples collected by special equipment. At monitoring station samples are created by pumping high volumes of air through glass fibre filter. In Finland there are 8 monitoring stations. By default all the monitoring stations are selected and the results of measurements are search from the last 720 hours. The default values can be overwritten by using the time and location related input parameters.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 geoid | int | Geoid of the location for which to return data. |  
 maxlocations | int | Amount of locations |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Latest dose rate of external radiation in Finland
__stuk::observations::external-radiation::latest::multipointcoverage__

    This stored query return the latest results of the external dose rate measured by the automatic dose rate monitoring stations in Finland. The automatic dose rate monitoring network have about 255 monitoring stations distributed evenly around the Finland.  The monitoring network is maintained by Radiation and Nuclear Safety Authority (STUK). By default, the latest data is searched from the last 24 hours. The data is returned as a multipointcoverage format. The default values can be overwritten by using the time and location related input parameters.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 geoid | int | Geoid of the location for which to return data. |  
 maxlocations | int | Amount of locations |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Latest dose rate of external radiation in Finland
__stuk::observations::external-radiation::latest::simple__

    This stored query return the latest dose rate of external radiation in Finland. The dose rate of external radiation is measured by an automatic external-dose rate-monitoring network maintained by Radiation and Nuclear Safety Authority (STUK) and local rescue services. The network comprises about 255 stations. By default, the latest data is searched from the last 24 hours. The data is returned as a simple format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 parameters | NameList | Parameters to return |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 geoid | int | Geoid of the location for which to return data. |  
 maxlocations | int | Amount of locations |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Dose rate of external radiation in Finland
__stuk::observations::external-radiation::multipointcoverage__

    This stored query return the results of the external dose rate measured by the automatic dose rate monitoring stations in Finland. The automatic dose rate monitoring network have about 255 monitoring stations distributed evenly around the Finland.  The monitoring network is maintained by Radiation and Nuclear Safety Authority (STUK). By default, the data is returned from the last 2 hours. The data is returned as a multipointcoverage format. The default values can be overwritten by using the time and location related input parameters.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 geoid | int | Geoid of the location for which to return data. |  
 maxlocations | int | Amount of locations |  
 crs | xsi:string | Coordinate projection to use in results |  |





## Hourly Air Quality Observations
__urban::observations::airquality::hourly::multipointcoverage__

    Hourly air quality observations from Finnish municipalities. By default, all the station are selected and the data is returned from the last 24 hours. The data is returned as multi point coverage format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  |





## Hourly Air Quality Observations
__urban::observations::airquality::hourly::simple__

    Hourly air quality observations from Finnish municipalities. By default, all the station are selected and the data is returned from the last 24 hours. The data is returned as a simple feature format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## Hourly Air Quality Observations
__urban::observations::airquality::hourly::timevaluepair__

    Hourly air quality observations from Finnish municipalities. By default, all the station are selected and the data is returned from the last 24 hours. The data is returned as timevaluepair format.
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| starttime | dateTime | Begin of the time interval |  
 endtime | dateTime | End of time interval |  
 timestep | int | The time step of data in minutes |  
 parameters | NameList | Parameters to return |  
 crs | xsi:string | Coordinate projection to use in results |  
 bbox | xsi:string | Bounding box of area for which to return data. |  
 place | xsi:string | The location for which to provide data |  
 fmisid | int | FMI observation station identifier. |  
 maxlocations | int | Amount of locations |  
 geoid | int | Geoid of the location for which to return data. |  
 timezone | xsi:string | Time zone |  |





## GetFeatureById
__urn:ogc:def:query:OGC-WFS::GetFeatureById__

    The GetFeatureById stored query is mandatory by WFS 2.0 spec.
    In the FMI case it's mostly useless however, because most of the
    features only have temporary IDs that are generated on-the-fly
    during the response generation, and thus cannot be used as permanent
    identifiers for those features
    
### Parameters

| Name | Type | Title | Abstract |
| --- | --- | --- | --- |
| id | xsi:string | Stored Query ID |  |

