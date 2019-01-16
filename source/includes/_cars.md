# Cars

## Create a Car

```shell
curl "https://hymer.ptchr-lv.nl/api/v1/car/create
    -X POST
    -H "Authorization: Bearer <your_access_token>"
    -H "Content-Type: application/json"
    -H "Accept: application/json"
    --data {
       "advertiser_id": 1,
       "license_plate_number": "aa-bb-cc",
       "chassis_number": null,
       "brand": "hymer",
       "type": "Exsis-t",      
       "serie": "T 647 Premium",
       "description": "Met de nieuwe Exsis-t zetten wij de succesvolle geschiedenis van de lichtgewichten voort. Met een totaal gewicht van minder dan 2.900 kg combineren wij in deze reeks lichtgewichtbouw en comfort op bijna perfecte wijze. De Exsis-t 588 weegt klaar voor vertrek slechts 2.770 kg, zodat u zonder problemen nog voldoende bagage kunt laden zonder de belangrijke grens van 3,5 ton te overschrijden. Hiermee zet hij opnieuw maatstaven uit in de klasse van de half-integralen. Dankzij speciaal ontwikkelde materialen, uiterst moderne productietechnieken, de GFK-lichtgewichtvloer, het AL-KO-lichtgewichtframe en de voor het merk typische PUAL-constructie konden we bij de productie van de Exsis-t veel gewicht besparen – zonder ons daarvoor op het vlak van uitrusting met minder tevreden te stellen: led-verlichting binnen, garagedeuren aan beide zijkanten en koudschuimmatrassen met verschillende zones zijn evenzeer standaard als het omvangrijke veiligheidspakket met airbags, ESP, Hill Holder en veel meer.",
       "body_type": "AL",
       "sleep_accomodations": "3",
       "beds":"2",
       "interior_layout":"FB",
       "headroom" : "0",
       "height" : "277",
       "length" : "744",
       "fuel_type": "B",
       "fuel_consumption_city": "16",
       "fuel_consumption_highway": "23",
       "fuel_consumption_combined": "20",
       "transmission_type": "H",
       "transmission_amount": 5,
       "color": "Zilver",
       "color_brand": null,
       "mileage": 59638,
       "mileage_type": "KM",
       "nap_valid": false,
       "engine_cylinders": 4,
       "engine_capacity": 1600,
       "engine_power": 74,
       "engine_power_type": "KW",
       "engine_top_speed": 180,
       "engine_top_speed_type": "KM",
       "emission_co2": 120,
       "load_capacity": 577,
       "doors": 5,
       "seats": 5,
       "keys_amount": 2,
       "weight": 4000,
       "construction_date": "2014-01-01",
       "apk_due_date": "2018-11-26",
       "apk_on_delivery": true,
       "price_excl_vat": 10450,
       "price_incl_vat": 10450,
       "price_delivery": 0,
       "price_bpm": 1051,
       "tax_benefit": 25,
       "tax_road_min": "117.00",
       "tax_road_max": "130.00",
       "tax_declarable" : true,
       "accessories": [
           ["3e remlicht","sec"],
           ["Airbag(s) hoofd en side","int"],
           ["Airbag bestuurder en passagier","sec"],
           ["Airco","int"],
           ["Alarm klasse 1(startblokkering)","sec"],
           ["Anti blokkeer systeem","sec"],
           ["AUX-ingang","int"],
           ["Bestuurdersstoel in hoogte verstelbaar","int"],
           ["Boordcomputer","int"],
           ["Buitenspiegels elektrisch verstelbaar","ext"],
           ["Centrale deurvergrendeling met afstandsbediening","ext"],
           ["Cruise control","int"],
           ["Electronic stability program","int"],
           ["Elektrische ramen voor","int"],
           ["Extra getint glas","int"],
           ["Hoofdsteunen achter","int"],
           ["Lederen stuurwiel","int"],
           ["Lichtmetalen velgen 16\"","ext"],
           ["Mistlampen voor","ext"],
           ["Multimedia-voorbereiding","int"],
           ["Navigatie systeem af fabriek","int"],
           ["Radio-cd/mp3 speler","int"],
           ["Ruitenwisser achter","ext"],
           ["Stuur verstelbaar","int"],
           ["USB-poort", "int"]
       ],
       "videos": [
           {
               "type": "YT",
               "url": "https://www.youtube.com/v/L3dqNPkBtnw"
           }
       ],
       "images": [
        "https://www.hymer.com/assets/images/modell-2018/reisemobile/exsis-t/HYMER_Exsis_t_silber_schwarz_Exterieur_Frontansicht.jpg"
       ]
   }
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": 3,
        "advertiser": {
            "id": 1,
            "name": "Autobedrijf Janssen",
            "street": "Stationstraat",
            "number": "10",
            "number_extra": "a",
            "zipcode": "1234AB",
            "city": "Maastricht",
            "country": "Nederland",
            "phone": "+31 40 123 45 67",
            "email": "info@autobedrijfjassen.nl",
            "web": "http://autobedrijfjanssen.nl",
            "created_at": "16-01-2019 14:14:46",
            "updated_at": "16-01-2019 14:14:46"
        },
        "license_plate_number": "aa-bb-cc",
        "chassis_number": null,
        "brand": "Hymer",
        "type": "Exsis-t",
        "serie": "T 647 Premium",
        "description": "Met de nieuwe Exsis-t zetten wij de succesvolle geschiedenis van de lichtgewichten voort. Met een totaal gewicht van minder dan 2.900 kg combineren wij in deze reeks lichtgewichtbouw en comfort op bijna perfecte wijze. De Exsis-t 588 weegt klaar voor vertrek slechts 2.770 kg, zodat u zonder problemen nog voldoende bagage kunt laden zonder de belangrijke grens van 3,5 ton te overschrijden. Hiermee zet hij opnieuw maatstaven uit in de klasse van de half-integralen. Dankzij speciaal ontwikkelde materialen, uiterst moderne productietechnieken, de GFK-lichtgewichtvloer, het AL-KO-lichtgewichtframe en de voor het merk typische PUAL-constructie konden we bij de productie van de Exsis-t veel gewicht besparen &ndash; zonder ons daarvoor op het vlak van uitrusting met minder tevreden te stellen: led-verlichting binnen, garagedeuren aan beide zijkanten en koudschuimmatrassen met verschillende zones zijn evenzeer standaard als het omvangrijke veiligheidspakket met airbags, ESP, Hill Holder en veel meer.",
        "body_type": null,
        "fuel_type": null,
        "fuel_consumption_city": "16",
        "fuel_consumption_highway": "23",
        "fuel_consumption_combined": "20",
        "transmission_type": null,
        "transmission_amount": 5,
        "color": "Zilver",
        "color_brand": null,
        "mileage": 59638,
        "mileage_type": "KM",
        "nap_valid": false,
        "engine_cylinders": 4,
        "engine_capacity": 1600,
        "engine_power": 74,
        "engine_power_type": "KW",
        "engine_top_speed": 180,
        "engine_top_speed_type": "KM",
        "emission_co2": 120,
        "load_capacity": 577,
        "doors": 5,
        "seats": 5,
        "keys_amount": 2,
        "weight": 4000,
        "construction_date": {
            "date": "2014-01-01 00:00:00.000000",
            "timezone_type": 3,
            "timezone": "Europe/Amsterdam"
        },
        "condition": null,
        "tax_declarable": null,
        "sleep_accomodations": "3",
        "beds": "2",
        "interior_layout": "FB",
        "headroom": "0",
        "height": "277",
        "length": "744",
        "apk_due_date": {
            "date": "2018-11-26 00:00:00.000000",
            "timezone_type": 3,
            "timezone": "Europe/Amsterdam"
        },
        "price_excl_vat": 10450,
        "price_incl_vat": 10450,
        "price_delivery": 0,
        "price_bpm": 1051,
        "tax_benefit": 25,
        "tax_road_min": "117.00",
        "tax_road_max": "130.00",
        "accessories": [
            {
                "name": "3e remlicht",
                "category": "sec"
            },
            {
                "name": "Airbag(s) hoofd en side",
                "category": "int"
            },
            {
                "name": "Airbag bestuurder en passagier",
                "category": "sec"
            },
            {
                "name": "Airco",
                "category": "int"
            },
            {
                "name": "Alarm klasse 1(startblokkering)",
                "category": "sec"
            },
            {
                "name": "Anti blokkeer systeem",
                "category": "sec"
            },
            {
                "name": "AUX-ingang",
                "category": "int"
            },
            {
                "name": "Bestuurdersstoel in hoogte verstelbaar",
                "category": "int"
            },
            {
                "name": "Boordcomputer",
                "category": "int"
            },
            {
                "name": "Buitenspiegels elektrisch verstelbaar",
                "category": "ext"
            },
            {
                "name": "Centrale deurvergrendeling met afstandsbediening",
                "category": "ext"
            },
            {
                "name": "Cruise control",
                "category": "int"
            },
            {
                "name": "Electronic stability program",
                "category": "int"
            },
            {
                "name": "Elektrische ramen voor",
                "category": "int"
            },
            {
                "name": "Extra getint glas",
                "category": "int"
            },
            {
                "name": "Hoofdsteunen achter",
                "category": "int"
            },
            {
                "name": "Lederen stuurwiel",
                "category": "int"
            },
            {
                "name": "Lichtmetalen velgen 16\"",
                "category": "ext"
            },
            {
                "name": "Mistlampen voor",
                "category": "ext"
            },
            {
                "name": "Multimedia-voorbereiding",
                "category": "int"
            },
            {
                "name": "Navigatie systeem af fabriek",
                "category": "int"
            },
            {
                "name": "Radio-cd/mp3 speler",
                "category": "int"
            },
            {
                "name": "Ruitenwisser achter",
                "category": "ext"
            },
            {
                "name": "Stuur verstelbaar",
                "category": "int"
            },
            {
                "name": "USB-poort",
                "category": "int"
            }
        ],
        "videos": [
            {
                "type": "YT",
                "url": "https://www.youtube.com/v/L3dqNPkBtnw"
            }
        ],
        "images": [],
        "created_at": "16-01-2019 14:51:41",
        "updated_at": "16-01-2019 14:51:41",
        "url": "https://hymer.ptchr-lv.nl/hymer-exsis-t-t-647-premium-1"
    }
}
```

This endpoint creates a new Car.

<aside class="warning">Make sure you send the json payload as raw body data to the endpoint. Also remember that the advertiser ID should be equal to the ID returned by your call when creating an Advertiser!</aside>

### HTTP Request

`POST https://hymer.ptchr-lv.nl/api/v1/car/create`

### Raw Body Parameters (JSON)

Parameter | Description | Required | Validation
--------- | ----------- | -------- | ----------
advertiser_id | The ID a given by the Advertiser endpoint | Yes | *existing ID as returned by Advertiser endpoint*
license_plate_number | The license plate number | Yes | 
brand | The brand name | Yes | 
type | The type name | Yes | 
serie | The series description | Yes | 
description | Full car description | No | 
color | The color of the car | Yes | 
color_brand | The factory name of the color | No | 
fuel_type | The fuel type (see below) | Yes | *in: B,D,E,EB,ED,LPG,O*
fuel_consumption_city | Fuel consumption in the city in KM per Liter | No | *numeric*
fuel_consumption_highway | Fuel consumption on the highway in KM per Liter | No | *numeric*
fuel_consumption_combined | Fuel consumption average in KM per Liter | No | *numeric*
transmission_type | Transmission type (see below) | Yes | *in: H,A,O*
transmission_amount | The amount of gears | No | *integer*
body_type | The body type (see below) | Yes | *in: AL,IN,CA,FC,O*
sleep_accomodations | how many people can sleep in this vehicle | No | *integer*
beds | How many beds this vehicle has| No | *integer*
interior_layout | What type of interior layout (see below) | No | *in: FR, LB, DB, O*
headroom | Inside height of vehicle in cm, leave to 0 ( zero ) if not available| No | *integer*
height | height of vehicle in cm | No | *integer*
length | length of vehicle in cm | No | *integer*     
construction_date | The construction date | Yes | *date:Y-m-d*
mileage | The mileage amount | Yes | *integer*
mileage_type | The mileage type (see below) | Yes | *in: KM,M*
doors | The number of doors | No | *integer*
engine_cylinders | The number of cylinders | No | *integer*
engine_capacity | Engine capacity in cc | No | *integer*
engine_power | The power of the engine | Yes | *integer*
engine_power_type | The power type (see below) | Yes | *in: PK,KW*
engine_top_speed | The top speed of the vehicle | No | *integer*
engine_top_speed_type | The speed type (see below) | No | *in: KM,M*
apk_due_date | Due date for the yearly check-up | No | *date:Y-m-d*
apk_on_delivery | APK on delivery | No | *boolean*
nap_valid | Does the car have a valid NAP? | No | *boolean*
price_excl_vat | Pricing excl VAT | Yes | *numeric*
price_incl_vat | Pricing incl VAT | Yes | *numeric*
price_delivery | Delivery costs | Yes | *numeric*
price_bpm | The BPM amount | No | *numeric*
chassis_number | The chassisnumber | No |
keys_amount | Amount of available keys | No | *integer*
emission_co2 | The co2 emission in g/km | No | *integer*
seats | The amount of seats | No | *integer*
load_capacity | The load capacity in Liter | No | *integer*
weight | The weight in kilogram | Yes | *integer*
tax_benefit | Tax benefit class in percent | No | *numeric*
road_tax_min | Minimum amount of road tax | Yes | *numeric*
road_tax_max | Maximum amount of road tax | Yes | *numeric*
tax_declarable | Is this vehicle tax declarable | No | *boolean*
images | Array of images (see below) | Yes | *array*
videos | Array of videos (see below) | No | *array*
accessories | Array of [accessories with categories] 'int', 'ext', 'sec', and 'O'. Interior, exterior, security and Overig. (see below) | No | *array[accesories, category]*

## Update a Car

```shell
curl "https://hymer.ptchr-lv.nl/api/v1/car/<ID>
    -X PUT
    -H "Authorization: Bearer <your_access_token>"
    -H "Content-Type: application/json"
    -H "Accept: application/json"
    --data{
       "advertiser_id": 1,
       "license_plate_number": "aa-bb-cc",
       "chassis_number": null,
       "brand": "hymer",
       "type": "Exsis-t",      
       "serie": "T 647 Premium",
       "description": "Met de nieuwe Exsis-t zetten wij de succesvolle geschiedenis van de lichtgewichten voort. Met een totaal gewicht van minder dan 2.900 kg combineren wij in deze reeks lichtgewichtbouw en comfort op bijna perfecte wijze. De Exsis-t 588 weegt klaar voor vertrek slechts 2.770 kg, zodat u zonder problemen nog voldoende bagage kunt laden zonder de belangrijke grens van 3,5 ton te overschrijden. Hiermee zet hij opnieuw maatstaven uit in de klasse van de half-integralen. Dankzij speciaal ontwikkelde materialen, uiterst moderne productietechnieken, de GFK-lichtgewichtvloer, het AL-KO-lichtgewichtframe en de voor het merk typische PUAL-constructie konden we bij de productie van de Exsis-t veel gewicht besparen – zonder ons daarvoor op het vlak van uitrusting met minder tevreden te stellen: led-verlichting binnen, garagedeuren aan beide zijkanten en koudschuimmatrassen met verschillende zones zijn evenzeer standaard als het omvangrijke veiligheidspakket met airbags, ESP, Hill Holder en veel meer.",
       "body_type": "AL",
       "sleep_accomodations": "3",
       "beds":"2",
       "interior_layout":"FB",
       "headroom" : "50",
       "height" : "277",
       "length" : "744",
       "fuel_type": "B",
       "fuel_consumption_city": "16",
       "fuel_consumption_highway": "23",
       "fuel_consumption_combined": "20",
       "transmission_type": "H",
       "transmission_amount": 5,
       "color": "Zilver",
       "color_brand": null,
       "mileage": 59638,
       "mileage_type": "KM",
       "nap_valid": false,
       "engine_cylinders": 4,
       "engine_capacity": 1600,
       "engine_power": 74,
       "engine_power_type": "KW",
       "engine_top_speed": 180,
       "engine_top_speed_type": "KM",
       "emission_co2": 120,
       "load_capacity": 577,
       "doors": 5,
       "seats": 5,
       "keys_amount": 2,
       "weight": 4000,
       "construction_date": "2014-01-01",
       "apk_due_date": "2018-11-26",
       "apk_on_delivery": true,
       "price_excl_vat": 10450,
       "price_incl_vat": 10450,
       "price_delivery": 0,
       "price_bpm": 1051,
       "tax_benefit": 25,
       "tax_road_min": "117.00",
       "tax_road_max": "130.00",
       "tax_declarable" : true,
       "accessories": [
           ["3e remlicht","sec"],
           ["Airbag(s) hoofd en side","int"],
           ["Airbag bestuurder en passagier","sec"],
           ["Airco","int"],
           ["Alarm klasse 1(startblokkering)","sec"],
           ["Anti blokkeer systeem","sec"],
           ["AUX-ingang","int"],
           ["Bestuurdersstoel in hoogte verstelbaar","int"],
           ["Boordcomputer","int"],
           ["Buitenspiegels elektrisch verstelbaar","ext"],
           ["Centrale deurvergrendeling met afstandsbediening","ext"],
           ["Cruise control","int"],
           ["Electronic stability program","int"],
           ["Elektrische ramen voor","int"],
           ["Extra getint glas","int"],
           ["Hoofdsteunen achter","int"],
           ["Lederen stuurwiel","int"],
           ["Lichtmetalen velgen 16\"","ext"],
           ["Mistlampen voor","ext"],
           ["Multimedia-voorbereiding","int"],
           ["Navigatie systeem af fabriek","int"],
           ["Radio-cd/mp3 speler","int"],
           ["Ruitenwisser achter","ext"],
           ["Stuur verstelbaar","int"],
           ["USB-poort", "int"]
       ],
       "videos": [
           {
               "type": "YT",
               "url": "https://www.youtube.com/v/L3dqNPkBtnw"
           }
       ],
       "images": [
        "https://www.hymer.com/assets/images/modell-2018/reisemobile/exsis-t/HYMER_Exsis_t_silber_schwarz_Exterieur_Frontansicht.jpg"
       ]
   }
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": 3,
        "advertiser": {
            "id": 1,
            "name": "Autobedrijf Janssen",
            "street": "Stationstraat",
            "number": "10",
            "number_extra": "a",
            "zipcode": "1234AB",
            "city": "Maastricht",
            "country": "Nederland",
            "phone": "+31 40 123 45 67",
            "email": "info@autobedrijfjassen.nl",
            "web": "http://autobedrijfjanssen.nl",
            "created_at": "16-01-2019 14:14:46",
            "updated_at": "16-01-2019 14:14:46"
        },
        "license_plate_number": "aa-bb-cc",
        "chassis_number": null,
        "brand": "Hymer",
        "type": "Exsis-t",
        "serie": "T 647 Premium",
        "description": "Met de nieuwe Exsis-t zetten wij de succesvolle geschiedenis van de lichtgewichten voort. Met een totaal gewicht van minder dan 2.900 kg combineren wij in deze reeks lichtgewichtbouw en comfort op bijna perfecte wijze. De Exsis-t 588 weegt klaar voor vertrek slechts 2.770 kg, zodat u zonder problemen nog voldoende bagage kunt laden zonder de belangrijke grens van 3,5 ton te overschrijden. Hiermee zet hij opnieuw maatstaven uit in de klasse van de half-integralen. Dankzij speciaal ontwikkelde materialen, uiterst moderne productietechnieken, de GFK-lichtgewichtvloer, het AL-KO-lichtgewichtframe en de voor het merk typische PUAL-constructie konden we bij de productie van de Exsis-t veel gewicht besparen &ndash; zonder ons daarvoor op het vlak van uitrusting met minder tevreden te stellen: led-verlichting binnen, garagedeuren aan beide zijkanten en koudschuimmatrassen met verschillende zones zijn evenzeer standaard als het omvangrijke veiligheidspakket met airbags, ESP, Hill Holder en veel meer.",
        "body_type": null,
        "fuel_type": null,
        "fuel_consumption_city": "16",
        "fuel_consumption_highway": "23",
        "fuel_consumption_combined": "20",
        "transmission_type": null,
        "transmission_amount": 5,
        "color": "Zilver",
        "color_brand": null,
        "mileage": 59638,
        "mileage_type": "KM",
        "nap_valid": false,
        "engine_cylinders": 4,
        "engine_capacity": 1600,
        "engine_power": 74,
        "engine_power_type": "KW",
        "engine_top_speed": 180,
        "engine_top_speed_type": "KM",
        "emission_co2": 120,
        "load_capacity": 577,
        "doors": 5,
        "seats": 5,
        "keys_amount": 2,
        "weight": 4000,
        "construction_date": {
            "date": "2014-01-01 00:00:00.000000",
            "timezone_type": 3,
            "timezone": "Europe/Amsterdam"
        },
        "condition": "N",
        "tax_declarable": null,
        "sleep_accomodations": "3",
        "beds": "2",
        "interior_layout": "FB",
        "headroom": "50",
        "height": "277",
        "length": "744",
        "apk_due_date": {
            "date": "2018-11-26 00:00:00.000000",
            "timezone_type": 3,
            "timezone": "Europe/Amsterdam"
        },
        "price_excl_vat": 10450,
        "price_incl_vat": 10450,
        "price_delivery": 0,
        "price_bpm": 1051,
        "tax_benefit": 25,
        "tax_road_min": "117.00",
        "tax_road_max": "130.00",
        "accessories": [
            {
                "name": "3e remlicht",
                "category": "sec"
            },
            {
                "name": "Airbag(s) hoofd en side",
                "category": "int"
            },
            {
                "name": "Airbag bestuurder en passagier",
                "category": "sec"
            },
            {
                "name": "Airco",
                "category": "int"
            },
            {
                "name": "Alarm klasse 1(startblokkering)",
                "category": "sec"
            },
            {
                "name": "Anti blokkeer systeem",
                "category": "sec"
            },
            {
                "name": "AUX-ingang",
                "category": "int"
            },
            {
                "name": "Bestuurdersstoel in hoogte verstelbaar",
                "category": "int"
            },
            {
                "name": "Boordcomputer",
                "category": "int"
            },
            {
                "name": "Buitenspiegels elektrisch verstelbaar",
                "category": "ext"
            },
            {
                "name": "Centrale deurvergrendeling met afstandsbediening",
                "category": "ext"
            },
            {
                "name": "Cruise control",
                "category": "int"
            },
            {
                "name": "Electronic stability program",
                "category": "int"
            },
            {
                "name": "Elektrische ramen voor",
                "category": "int"
            },
            {
                "name": "Extra getint glas",
                "category": "int"
            },
            {
                "name": "Hoofdsteunen achter",
                "category": "int"
            },
            {
                "name": "Lederen stuurwiel",
                "category": "int"
            },
            {
                "name": "Lichtmetalen velgen 16\"",
                "category": "ext"
            },
            {
                "name": "Mistlampen voor",
                "category": "ext"
            },
            {
                "name": "Multimedia-voorbereiding",
                "category": "int"
            },
            {
                "name": "Navigatie systeem af fabriek",
                "category": "int"
            },
            {
                "name": "Radio-cd/mp3 speler",
                "category": "int"
            },
            {
                "name": "Ruitenwisser achter",
                "category": "ext"
            },
            {
                "name": "Stuur verstelbaar",
                "category": "int"
            },
            {
                "name": "USB-poort",
                "category": "int"
            }
        ],
        "videos": [
            {
                "type": "YT",
                "url": "https://www.youtube.com/v/L3dqNPkBtnw"
            }
        ],
        "images": [
            "https://www.hymer.com/assets/images/modell-2018/reisemobile/exsis-t/HYMER_Exsis_t_silber_schwarz_Exterieur_Frontansicht.jpg"
        ],
        "created_at": "16-01-2019 14:51:41",
        "updated_at": "16-01-2019 14:54:39",
        "url": "https://hymer.ptchr-lv.nl/hymer-exsis-t-t-647-premium-1"
    }
}
```

This endpoint updates an existing Car.

<aside class="warning">Make sure you send the json payload as raw body data to the endpoint.</aside>

### HTTP Request

`PUT https://hymer.ptchr-lv.nl/api/v1/car/<ID>`

### Raw Body Parameters (JSON)

Parameter | Description | Required | Validation
--------- | ----------- | -------- | ----------
advertiser_id | The ID a given by the Advertiser endpoint | Yes | *existing ID as returned by Advertiser endpoint*
license_plate_number | The license plate number | Yes | 
brand | The brand name | Yes | 
type | The type name | Yes | 
sleep_accomodations | how many people can sleep in this vehicle | No | *integer*
beds | How many beds this vehicle has| No | *integer*
interior_layout | What type of interior layout (see below) | No | *in: FR, LB, DB, O*
headroom | Inside height of vehicle in cm| No | *integer*
height | height of vehicle in cm | No | *integer*
length | length of vehicle in cm | No | *integer* 
serie | The series description | Yes | 
description | Full car description | No | 
color | The color of the car | Yes | 
color_brand | The factory name of the color | No | 
fuel_type | The fuel type (see below) | Yes | *in: B,D,E,EB,ED,LPG,O*
fuel_consumption_city | Fuel consumption in the city in KM per Liter | No | *numeric*
fuel_consumption_highway | Fuel consumption on the highway in KM per Liter | No | *numeric*
fuel_consumption_combined | Fuel consumption average in KM per Liter | No | *numeric*
transmission_type | Transmission type (see below) | Yes | *in: H,A,O*
transmission_amount | The amount of gears | No | *integer*
body_type | The body type (see below) | Yes | *in: AL,IN,CA,FC,O*
construction_date | The construction date | Yes | *date:Y-m-d*
mileage | The mileage amount | Yes | *integer*
mileage_type | The mileage type (see below) | Yes | *in: KM,M*
doors | The number of doors | No | *integer*
engine_cylinders | The number of cylinders | No | *integer*
engine_capacity | Engine capacity in cc | No | *integer*
engine_power | The power of the engine | Yes | *integer*
engine_power_type | The power type (see below) | Yes | *in: PK,KW*
engine_top_speed | The top speed of the vehicle | No | *integer*
engine_top_speed_type | The speed type (see below) | No | *in: KM,M*
apk_due_date | Due date for the yearly check-up | No | *date:Y-m-d*
apk_on_delivery | APK on delivery | No | *boolean*
nap_valid | Does the car have a valid NAP? | No | *boolean*
price_excl_vat | Pricing excl VAT | Yes | *numeric*
price_incl_vat | Pricing incl VAT | Yes | *numeric*
price_delivery | Delivery costs | Yes | *numeric*
price_bpm | The BPM amount | No | *numeric*
chassis_number | The chassisnumber | No |
keys_amount | Amount of available keys | No | *integer*
emission_co2 | The co2 emission in g/km | No | *integer*
seats | The amount of seats | No | *integer*
load_capacity | The load capacity in Liter | No | *integer*
weight | The weight in kilogram | Yes | *integer*
tax_benefit | Tax benefit class in percent | No | *numeric*
road_tax_min | Minimum amount of road tax | Yes | *numeric*
road_tax_max | Maximum amount of road tax | Yes | *numeric*
tax_declarable | Is this vehicle tax declarable | No | *boolean*
images | Array of images (see below) | Yes | *array*
videos | Array of videos (see below) | No | *array*
accessories | Array of [accessories with categories] 'int', 'ext', 'sec', and 'O'. Interior, exterior, security and Overig. (see below) | No | *array[accesories, category]*

## Get All Cars

```shell
curl "https://hymer.ptchr-lv.nl/api/v1/car"
  -H "Authorization: Bearer <your_access_token>"
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            /*full car response*/
        },
        {
            /*full car2 response*/
        }
    ]
}
```

This endpoint retrieves all Cars created by the currently authenticated client.

### HTTP Request

`GET https://hymer.ptchr-lv.nl/api/v1/car`

### Query Parameters

None

<aside class="success">
Remember — don't forget to authenticate!
</aside>

## Get a Specific Car

```shell
curl "https://hymer.ptchr-lv.nl/api/v1/car/2"
  -H "Authorization: Bearer <your_access_token>"
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": 2,
        "advertiser": {
            "id": 1,
            "name": "Autobedrijf Janssen",
            "street": "Stationstraat",
            "number": "10",
            "number_extra": "a",
            "zipcode": "1234AB",
            "city": "Maastricht",
            "country": "Nederland",
            "phone": "+31 40 123 45 67",
            "email": "info@autobedrijfjassen.nl",
            "web": "http://autobedrijfjanssen.nl",
            "created_at": "16-01-2019 14:14:46",
            "updated_at": "16-01-2019 14:14:46"
        },
        "license_plate_number": "aa-bb-cc",
        "chassis_number": null,
        "brand": "Hymer",
        "type": "Exsis-t",
        "serie": "T 647 Premium",
        "description": "Met de nieuwe Exsis-t zetten wij de succesvolle geschiedenis van de lichtgewichten voort. Met een totaal gewicht van minder dan 2.900 kg combineren wij in deze reeks lichtgewichtbouw en comfort op bijna perfecte wijze. De Exsis-t 588 weegt klaar voor vertrek slechts 2.770 kg, zodat u zonder problemen nog voldoende bagage kunt laden zonder de belangrijke grens van 3,5 ton te overschrijden. Hiermee zet hij opnieuw maatstaven uit in de klasse van de half-integralen. Dankzij speciaal ontwikkelde materialen, uiterst moderne productietechnieken, de GFK-lichtgewichtvloer, het AL-KO-lichtgewichtframe en de voor het merk typische PUAL-constructie konden we bij de productie van de Exsis-t veel gewicht besparen &ndash; zonder ons daarvoor op het vlak van uitrusting met minder tevreden te stellen: led-verlichting binnen, garagedeuren aan beide zijkanten en koudschuimmatrassen met verschillende zones zijn evenzeer standaard als het omvangrijke veiligheidspakket met airbags, ESP, Hill Holder en veel meer.",
        "body_type": null,
        "fuel_type": null,
        "fuel_consumption_city": 16,
        "fuel_consumption_highway": 23,
        "fuel_consumption_combined": 20,
        "transmission_type": null,
        "transmission_amount": 5,
        "color": "Zilver",
        "color_brand": null,
        "mileage": 59638,
        "mileage_type": "KM",
        "nap_valid": false,
        "engine_cylinders": 4,
        "engine_capacity": 1600,
        "engine_power": 74,
        "engine_power_type": "KW",
        "engine_top_speed": 180,
        "engine_top_speed_type": "KM",
        "emission_co2": 120,
        "load_capacity": 577,
        "doors": 5,
        "seats": 5,
        "keys_amount": 2,
        "weight": 4000,
        "construction_date": {
            "date": "2014-01-01 00:00:00.000000",
            "timezone_type": 3,
            "timezone": "Europe/Amsterdam"
        },
        "condition": "N",
        "tax_declarable": null,
        "sleep_accomodations": 3,
        "beds": 2,
        "interior_layout": "FB",
        "headroom": 0,
        "height": 277,
        "length": 744,
        "apk_due_date": {
            "date": "2018-11-26 00:00:00.000000",
            "timezone_type": 3,
            "timezone": "Europe/Amsterdam"
        },
        "price_excl_vat": "10450.00",
        "price_incl_vat": "10450.00",
        "price_delivery": "0.00",
        "price_bpm": "1051.00",
        "tax_benefit": 25,
        "tax_road_min": "117.00",
        "tax_road_max": "130.00",
        "accessories": [
            {
                "name": "3e remlicht",
                "category": "sec"
            },
            {
                "name": "Airbag(s) hoofd en side",
                "category": "int"
            },
            {
                "name": "Airbag bestuurder en passagier",
                "category": "sec"
            },
            {
                "name": "Airco",
                "category": "int"
            },
            {
                "name": "Alarm klasse 1(startblokkering)",
                "category": "sec"
            },
            {
                "name": "Anti blokkeer systeem",
                "category": "sec"
            },
            {
                "name": "AUX-ingang",
                "category": "int"
            },
            {
                "name": "Bestuurdersstoel in hoogte verstelbaar",
                "category": "int"
            },
            {
                "name": "Boordcomputer",
                "category": "int"
            },
            {
                "name": "Buitenspiegels elektrisch verstelbaar",
                "category": "ext"
            },
            {
                "name": "Centrale deurvergrendeling met afstandsbediening",
                "category": "ext"
            },
            {
                "name": "Cruise control",
                "category": "int"
            },
            {
                "name": "Electronic stability program",
                "category": "int"
            },
            {
                "name": "Elektrische ramen voor",
                "category": "int"
            },
            {
                "name": "Extra getint glas",
                "category": "int"
            },
            {
                "name": "Hoofdsteunen achter",
                "category": "int"
            },
            {
                "name": "Lederen stuurwiel",
                "category": "int"
            },
            {
                "name": "Lichtmetalen velgen 16\"",
                "category": "ext"
            },
            {
                "name": "Mistlampen voor",
                "category": "ext"
            },
            {
                "name": "Multimedia-voorbereiding",
                "category": "int"
            },
            {
                "name": "Navigatie systeem af fabriek",
                "category": "int"
            },
            {
                "name": "Radio-cd/mp3 speler",
                "category": "int"
            },
            {
                "name": "Ruitenwisser achter",
                "category": "ext"
            },
            {
                "name": "Stuur verstelbaar",
                "category": "int"
            },
            {
                "name": "USB-poort",
                "category": "int"
            }
        ],
        "videos": [
            {
                "type": "YT",
                "url": "https://www.youtube.com/v/L3dqNPkBtnw"
            }
        ],
        "images": [
            "https://www.hymer.com/assets/images/modell-2018/reisemobile/exsis-t/HYMER_Exsis_t_silber_schwarz_Exterieur_Frontansicht.jpg"
        ],
        "created_at": "16-01-2019 14:26:49",
        "updated_at": "16-01-2019 14:26:49",
        "url": "https://hymer.ptchr-lv.nl/hymer-exsis-t-t-647-premium"
    }
}
```

This endpoint retrieves a specific Car.

<aside class="warning">If you try to get an advertiser that wasn't added by your client a HTTP error will be returned.</aside>

### HTTP Request

`GET https://hymer.ptchr-lv.nl/api/v1/car/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the Car to retrieve

## Delete a Specific Car

```shell
curl "https://hymer.ptchr-lv.nl/api/v1/car/1"
  -X DELETE
  -H "Authorization: Bearer <your_access_token>"
```

> The above command returns JSON structured like this:

```json
[]
```

This endpoint deletes a specific Car.

<aside class="warning">The JSON response will be empty, when the Car is deleted succesfully a HTTP 200 OK response will be returned.</aside>

### HTTP Request

`DELETE https://hymer.ptchr-lv.nl/api/v1/car/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the Car to delete

## Field type description

Some fields have abbreviated values, below you can find what each value means.

### fuel_type

Value | Description
----- | -----------
B | Benzine
D | Diesel
E | Elektrisch
EB | Elektrisch-Benzine
ED | Elektisch-Diesel
LPG | LPG/Gas
O | Overige

### transmission_type

Value | Description
----- | -----------
H | Handgeschakeld
A | Automaat
O | Overige / semi-automaat

### body_type

Value | Description
----- | -----------
AL | Alkoof
IN | (Half) Integraal
CA | Caravans
FC | FamilieCaravans
O | Overige


### interior_layout

Value | Description
----- | -----------
FR | Frans Bed
LB | Lengte Bed
DB | Dwars Bed
O | Overige

### mileage_type

Value | Description
----- | -----------
KM | Kilometer
M | Mijl

### engine_power_type

Value | Description
----- | -----------
PK | PK/HP
KW | KW

### engine_top_speed_type

Value | Description
----- | -----------
KM | KM/u
M | M/h

### images

The images key in the body should contain an array holding all images, a sample payload is:

```json
{
    // other data
    "images": [
        {
            "url": "http://www.google.com"
        },
        {
            "url": "http://www.google.com"
        },
        {
            "url": "http://www.google.com"
        }
    ]
    // other data
}
```

### videos

The videos key in the body should contain an array holding all images, including the video type, a sample payload is:

```json
{
    // other data
    "videos": [
        {
            "type": "YT",
            "url": "http://www.youtube.com"
        },
        {
            "type": "VM",
            "url": "http://www.vimeo.com"
        }
    ]
    // other data
}
```

Accepted video types currently are `YT` (YouTube) and `VM` (Vimeo).

### accessories

The accessories key should contain an array holding all accessories with categories(int, ext, sec, o).
accessories | Array of [accessories with categories] 'int', 'ext', 'sec', and 'O'. Interior, exterior, security and Overig. (see below) | No | *array[accesories, category]*

a sample payload is:

```json
{
    // other data
    "accessories": [
      ["xenon", "ext"],
      ["sportstoelen", "int"], 
      ["climate control","int"],
      ["alarmsysteem", "sec"],
      ["lane-assist", "sec"]
    // other data
}
```