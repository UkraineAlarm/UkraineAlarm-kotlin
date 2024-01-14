# AlertsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiV3AlertsGet**](AlertsApi.md#apiV3AlertsGet) | **GET** /api/v3/alerts | Області, регіони та громади з тривогами
[**apiV3AlertsRegionHistoryGet**](AlertsApi.md#apiV3AlertsRegionHistoryGet) | **GET** /api/v3/alerts/regionHistory | Отримати останніх 25 тривог регіону
[**apiV3AlertsRegionIdGet**](AlertsApi.md#apiV3AlertsRegionIdGet) | **GET** /api/v3/alerts/{regionId} | Статус області/регіону/громади
[**apiV3AlertsStatusGet**](AlertsApi.md#apiV3AlertsStatusGet) | **GET** /api/v3/alerts/status | Перевірка номеру останньої дії. Використовувати для перевірки необхідності оновлювати дані

<a name="apiV3AlertsGet"></a>
# **apiV3AlertsGet**
> kotlin.Array&lt;AlertRegionModel&gt; apiV3AlertsGet()

Області, регіони та громади з тривогами

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = AlertsApi()
try {
    val result : kotlin.Array<AlertRegionModel> = apiInstance.apiV3AlertsGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AlertsApi#apiV3AlertsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AlertsApi#apiV3AlertsGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Array&lt;AlertRegionModel&gt;**](AlertRegionModel.md)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="apiV3AlertsRegionHistoryGet"></a>
# **apiV3AlertsRegionHistoryGet**
> kotlin.Array&lt;RegionAlarmsHistory&gt; apiV3AlertsRegionHistoryGet(regionId)

Отримати останніх 25 тривог регіону

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = AlertsApi()
val regionId : kotlin.String = regionId_example // kotlin.String | 
try {
    val result : kotlin.Array<RegionAlarmsHistory> = apiInstance.apiV3AlertsRegionHistoryGet(regionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AlertsApi#apiV3AlertsRegionHistoryGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AlertsApi#apiV3AlertsRegionHistoryGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **regionId** | **kotlin.String**|  | [optional]

### Return type

[**kotlin.Array&lt;RegionAlarmsHistory&gt;**](RegionAlarmsHistory.md)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="apiV3AlertsRegionIdGet"></a>
# **apiV3AlertsRegionIdGet**
> kotlin.Array&lt;AlertRegionModel&gt; apiV3AlertsRegionIdGet(regionId)

Статус області/регіону/громади

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = AlertsApi()
val regionId : kotlin.String = regionId_example // kotlin.String | ID області/регіону/громади
try {
    val result : kotlin.Array<AlertRegionModel> = apiInstance.apiV3AlertsRegionIdGet(regionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AlertsApi#apiV3AlertsRegionIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AlertsApi#apiV3AlertsRegionIdGet")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **regionId** | **kotlin.String**| ID області/регіону/громади |

### Return type

[**kotlin.Array&lt;AlertRegionModel&gt;**](AlertRegionModel.md)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="apiV3AlertsStatusGet"></a>
# **apiV3AlertsStatusGet**
> AlertModification apiV3AlertsStatusGet()

Перевірка номеру останньої дії. Використовувати для перевірки необхідності оновлювати дані

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = AlertsApi()
try {
    val result : AlertModification = apiInstance.apiV3AlertsStatusGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AlertsApi#apiV3AlertsStatusGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AlertsApi#apiV3AlertsStatusGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AlertModification**](AlertModification.md)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

