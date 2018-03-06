# Lithuania GeoJSON

Various level exports of lithuanian map into GeoJSON format.

Export is done from http://overpass-turbo.eu/

## Counties

```
[out:json][timeout:45];
area["ISO3166-1"="LT"]->.a;
(relation(area.a)["admin_level"=4][boundary="administrative"];);
out body;
>;
out skel qt;
```

![counties.png](images/counties.png)
