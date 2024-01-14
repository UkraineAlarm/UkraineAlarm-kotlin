# WebHookApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiV3WebhookDelete**](WebHookApi.md#apiV3WebhookDelete) | **DELETE** /api/v3/webhook | Відписка на WebHook про нові сирени та їх відбій
[**apiV3WebhookPatch**](WebHookApi.md#apiV3WebhookPatch) | **PATCH** /api/v3/webhook | Оновлення WebHook посилання про нові сирени та їх відбій
[**apiV3WebhookPost**](WebHookApi.md#apiV3WebhookPost) | **POST** /api/v3/webhook | Підписка на WebHook про нові сирени та їх відбій. У вебхукі відпрявляється подія тривоги/відбою (приклад в відповіді \&quot;200\&quot;)

<a name="apiV3WebhookDelete"></a>
# **apiV3WebhookDelete**
> apiV3WebhookDelete(body)

Відписка на WebHook про нові сирени та їх відбій

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = WebHookApi()
val body : WebHookModel =  // WebHookModel | 
try {
    apiInstance.apiV3WebhookDelete(body)
} catch (e: ClientException) {
    println("4xx response calling WebHookApi#apiV3WebhookDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebHookApi#apiV3WebhookDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**WebHookModel**](WebHookModel.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: Not defined

<a name="apiV3WebhookPatch"></a>
# **apiV3WebhookPatch**
> apiV3WebhookPatch(body)

Оновлення WebHook посилання про нові сирени та їх відбій

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = WebHookApi()
val body : WebHookModel =  // WebHookModel | 
try {
    apiInstance.apiV3WebhookPatch(body)
} catch (e: ClientException) {
    println("4xx response calling WebHookApi#apiV3WebhookPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebHookApi#apiV3WebhookPatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**WebHookModel**](WebHookModel.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: Not defined

<a name="apiV3WebhookPost"></a>
# **apiV3WebhookPost**
> AlertRegionModel apiV3WebhookPost(body)

Підписка на WebHook про нові сирени та їх відбій. У вебхукі відпрявляється подія тривоги/відбою (приклад в відповіді \&quot;200\&quot;)

### Example
```kotlin
// Import classes:
//import UkraineAlarm.infrastructure.*
//import io.swagger.client.models.*;

val apiInstance = WebHookApi()
val body : WebHookModel =  // WebHookModel | 
try {
    val result : AlertRegionModel = apiInstance.apiV3WebhookPost(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebHookApi#apiV3WebhookPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebHookApi#apiV3WebhookPost")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**WebHookModel**](WebHookModel.md)|  | [optional]

### Return type

[**AlertRegionModel**](AlertRegionModel.md)

### Authorization

[Token](../README.md#Token)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

