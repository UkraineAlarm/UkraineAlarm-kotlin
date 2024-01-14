# RegionsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiV3RegionsGet**](RegionsApi.md#apiV3RegionsGet) | **GET** /api/v3/regions | Повертає список усіх областей, регіонів та міст

<a name="apiV3RegionsGet"></a>
# **apiV3RegionsGet**
> RegionsViewModel apiV3RegionsGet()

Повертає список усіх областей, регіонів та міст

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = RegionsApi()
try {
    val result : RegionsViewModel = apiInstance.apiV3RegionsGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RegionsApi#apiV3RegionsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RegionsApi#apiV3RegionsGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**RegionsViewModel**](RegionsViewModel.md)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

