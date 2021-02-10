# Sky Quality Observed

**Work in progress**

## Description

An observation of sky quality conditions - light pollution - at a certain place and time.

## Data Model



-   `id` : Unique identifier.
-   `type` : Entity type. It must be equal to `SkyQualityObserved`.


-   `name` : An  name for this item
    -   Attribute type: Property. [Text](https://schema.org/Text)
    -   Optional

-   `alternateName` : An alternative name for this item
    -   Attribute type: Property. [Text](https://schema.org/Text)
    -   Optional

-   `description` : An alternative name for this item
    -   Attribute type: Property. [Text](https://schema.org/Text)
    -   Optional

-   `location` : Phisical location for the item.
    -   Attribute type: Property
    -   Optional

-   `address` : The mailing address.
    -   Attribute type: Property
    -   Optional

-   `areaServed` : Higher level area to which this sky quality measurement belongs to. It
    can be used to group sky quality measurements per district, neighbourhood, etc.
    -   Attribute type: Property. [Text](https://schema.org/Text)
    -   Normative References:
        [https://schema.org/areaServed](https://schema.org/areaServed)
    -   Optional

-   `skyQualityLevel` : Overall qualitative level of sky quality 
    corresponding to the [Bortle scale.](https://en.wikipedia.org/wiki/Bortle_scale)
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `skyQuality` : Overall quantitative level of sky quality in 
	Magnitudes per Square Arc Second (mag/arcsec^2) using the standard SQ filter 
	Hoya CM500.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Magnitudes per Square Arc Second (mag/arcsec^2)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `skyQuality_B` : Overall quantitative level of sky quality in 
	Magnitudes per Square Arc Second (mag/arcsec^2) using a B photometric filter
	Johnson-Cousins.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Magnitudes per Square Arc Second (mag/arcsec^2)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `skyQuality_V` : Overall quantitative level of sky quality in 
	Magnitudes per Square Arc Second (mag/arcsec^2) using a V photometric filter
	Johnson-Cousins.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Magnitudes per Square Arc Second (mag/arcsec^2)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `skyQuality_R` : Overall quantitative level of sky quality in 
	Magnitudes per Square Arc Second (mag/arcsec^2) using a R photometric filter
	Johnson-Cousins.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Magnitudes per Square Arc Second (mag/arcsec^2)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `frequency` : Raw frequency output from photomer using the standard SQ filter 
	Hoya CM500.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Hertz (Hz)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `frequency_B` : Raw frequency output from photomer using a B photometric filter
	Johnson-Cousins.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Hertz (Hz)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `frequency_V` : Raw frequency output from photomer using a V photometric filter
	Johnson-Cousins.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Hertz (Hz)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `frequency_R` : Raw frequency output from photomer using a R photometric filter
	Johnson-Cousins.
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Hertz (Hz)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `ambientTemperature` : Ambient temperature measured by the device
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Celsius degrees (ºC)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `skyTemperature` : Sky temperature - clouds - measured by the device
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: Celsius degrees (ºC)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional

-   `cloudCoverage` : Cloud coverage using [Okta](https://en.wikipedia.org/wiki/Okta) scale
    -   Attribute type: Property. [Number](https://schema.org/Number)
    -	Default unit: [Okta](https://en.wikipedia.org/wiki/Okta)
    -   Attribute metadata:
        -   `timestamp` : optional timestamp for the observed value in ISO8601
            format. It can be omitted if the observation time is the same as the one
            captured by the `dateObserved` attribute at entity level.
            -   Type: [DateTime](https://schema.org/DateTime)
    -   Optional



## Examples

### Normalized Example

Normalized NGSI response


```json

```


### key-value pairs Example

Sample uses simplified representation for data consumers `?options=keyValues`

```json
{
	"id":"NightEye:001",
	"type":"SkyObserved",
	"name":"Sky Quality Station 0001",
	"alternateName":"Cerro de los vientos",
	"description":"NightEye Sky Quality observation at Cerro de los vientos",
	"location":"GeoJSON",
	"address":{
		"streetAddress": "Calle Cerro de los vientos",  
		"addressLocality": "Algeciras",  
		"addressCountry": "Spain"
	},
	"areaServed":0,
	"skyQualityLevel":0,
	"skyQuality":21.73,
	"skyQuality_B":21.54,
	"skyQuality_V":21.43,
	"skyQuality_R":21.33,
	"frequency":7443,
	"frequency_B":7567,
	"frequency_V":7632,
	"frequency_R":7932,
	"ambientTemperature":18.45,
	"skyTemperature":-18.04,
	"cloudCoverage":4,
}
```


### LD Example

Sample uses the NGSI-LD representation

```json

```