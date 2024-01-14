# UkraineAlarm - Kotlin library for the [Ukraine Alert API](https://api.ukrainealarm.com/)

## Requires

* Kotlin 1.4.30
* Gradle 5.3

## Build

First, create the gradle wrapper script:

```
gradle wrapper
```

Then, run:

```
./gradlew check assemble
```

This runs all tests and packages the library.

## Features/Implementation Notes

* Supports JSON inputs/outputs, File inputs, and Form inputs.
* Supports collection formats for query parameters: csv, tsv, ssv, pipes.
* Some Kotlin and Java types are fully qualified to avoid conflicts with types defined in Swagger definitions.
* Implementation of ApiClient is intended to reduce method counts, specifically to benefit Android targets.

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to */*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AlertsApi* | [**apiV3AlertsGet**](docs/AlertsApi.md#apiv3alertsget) | **GET** /api/v3/alerts | Області, регіони та громади з тривогами
*AlertsApi* | [**apiV3AlertsRegionHistoryGet**](docs/AlertsApi.md#apiv3alertsregionhistoryget) | **GET** /api/v3/alerts/regionHistory | Отримати останніх 25 тривог регіону
*AlertsApi* | [**apiV3AlertsRegionIdGet**](docs/AlertsApi.md#apiv3alertsregionidget) | **GET** /api/v3/alerts/{regionId} | Статус області/регіону/громади
*AlertsApi* | [**apiV3AlertsStatusGet**](docs/AlertsApi.md#apiv3alertsstatusget) | **GET** /api/v3/alerts/status | Перевірка номеру останньої дії. Використовувати для перевірки необхідності оновлювати дані
*RegionsApi* | [**apiV3RegionsGet**](docs/RegionsApi.md#apiv3regionsget) | **GET** /api/v3/regions | Повертає список усіх областей, регіонів та міст
*WebHookApi* | [**apiV3WebhookDelete**](docs/WebHookApi.md#apiv3webhookdelete) | **DELETE** /api/v3/webhook | Відписка на WebHook про нові сирени та їх відбій
*WebHookApi* | [**apiV3WebhookPatch**](docs/WebHookApi.md#apiv3webhookpatch) | **PATCH** /api/v3/webhook | Оновлення WebHook посилання про нові сирени та їх відбій
*WebHookApi* | [**apiV3WebhookPost**](docs/WebHookApi.md#apiv3webhookpost) | **POST** /api/v3/webhook | Підписка на WebHook про нові сирени та їх відбій. У вебхукі відпрявляється подія тривоги/відбою (приклад в відповіді \"200\")

<a name="documentation-for-models"></a>
## Documentation for Models

 - [io.swagger.client.models.Alert](docs/Alert.md)
 - [io.swagger.client.models.AlertModification](docs/AlertModification.md)
 - [io.swagger.client.models.AlertRegionModel](docs/AlertRegionModel.md)
 - [io.swagger.client.models.AlertType](docs/AlertType.md)
 - [io.swagger.client.models.RegionAlarmModel](docs/RegionAlarmModel.md)
 - [io.swagger.client.models.RegionAlarmsHistory](docs/RegionAlarmsHistory.md)
 - [io.swagger.client.models.RegionViewModel](docs/RegionViewModel.md)
 - [io.swagger.client.models.RegionsViewModel](docs/RegionsViewModel.md)
 - [io.swagger.client.models.TimeSpan](docs/TimeSpan.md)
 - [io.swagger.client.models.V2RegionType](docs/V2RegionType.md)
 - [io.swagger.client.models.WebHookModel](docs/WebHookModel.md)

<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="Token"></a>
### Token


