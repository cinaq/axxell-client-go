# \DefaultApi

All URIs are relative to *https://axxell.cinaq.com/v1/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AggregateCountEvents**](DefaultApi.md#AggregateCountEvents) | **Get** /aggregates/countevents/{eventType} | 
[**AggregateEffective**](DefaultApi.md#AggregateEffective) | **Get** /aggregates/effective/{eventType} | 
[**AggregateEvents**](DefaultApi.md#AggregateEvents) | **Get** /aggregates/events/{eventType} | 
[**AggregateRecent**](DefaultApi.md#AggregateRecent) | **Get** /aggregates/recent/{eventType} | 
[**AggregateTop**](DefaultApi.md#AggregateTop) | **Get** /aggregates/top/{eventType} | 
[**AuthStore**](DefaultApi.md#AuthStore) | **Post** /auth | 
[**DeleteAllEvents**](DefaultApi.md#DeleteAllEvents) | **Delete** /events | 
[**DeleteAllItems**](DefaultApi.md#DeleteAllItems) | **Delete** /items | 
[**DeleteItem**](DefaultApi.md#DeleteItem) | **Delete** /items/{itemid} | 
[**RecommendInteresting**](DefaultApi.md#RecommendInteresting) | **Get** /recommendations/interesting | 
[**RecommendSimilar**](DefaultApi.md#RecommendSimilar) | **Get** /recommendations/similar | 
[**RegisterEvent**](DefaultApi.md#RegisterEvent) | **Post** /events | 
[**RegisterItem**](DefaultApi.md#RegisterItem) | **Post** /items | 
[**RegisterStore**](DefaultApi.md#RegisterStore) | **Post** /store | 
[**RetrieveEvents**](DefaultApi.md#RetrieveEvents) | **Get** /events | 
[**RetrieveItems**](DefaultApi.md#RetrieveItems) | **Get** /items | 


# **AggregateCountEvents**
> DataPoint AggregateCountEvents($storeid, $eventType, $dataPeriod)



Return list of counts per event


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **eventType** | **string**| Valid values purchase, view or recommend | 
 **dataPeriod** | **string**| Valid values are last7days, last30days, today, yesterday | 

### Return type

[**DataPoint**](DataPoint.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AggregateEffective**
> []DataPoint AggregateEffective($storeid, $eventType)



Return list of aggregated data points correlated with recommendationa and eventType


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **eventType** | **string**| Valid values purchase, view or recommend | 

### Return type

[**[]DataPoint**](DataPoint.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AggregateEvents**
> []DataPoint AggregateEvents($storeid, $eventType)



Return list of aggregated data points


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **eventType** | **string**| Valid values purchase, view or recommend | 

### Return type

[**[]DataPoint**](DataPoint.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AggregateRecent**
> []Item AggregateRecent($storeid, $eventType)



Returns recent products


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **eventType** | **string**| Valid values purchase, view or recommend | 

### Return type

[**[]Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AggregateTop**
> []Item AggregateTop($storeid, $eventType)



Returns top products


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **eventType** | **string**| Valid values purchase, view or recommend | 

### Return type

[**[]Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AuthStore**
> Store AuthStore($store)



Retrieve authentication token using password


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **store** | [**Store**](Store.md)| Store | 

### Return type

[**Store**](Store.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAllEvents**
> Event DeleteAllEvents($storeid)



Delete all events


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 

### Return type

[**Event**](Event.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAllItems**
> Item DeleteAllItems($storeid)



Delete all items


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 

### Return type

[**Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteItem**
> Item DeleteItem($storeid, $itemid)



Delete existing item


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **itemid** | **string**| Item identifier | 

### Return type

[**Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RecommendInteresting**
> []Item RecommendInteresting($storeid, $userid, $count)



Return list of recommended items


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **userid** | **string**| Interesting items for visitor | 
 **count** | **float64**| Return exactly this amount of suggestions. Maximum value is 50, default is 5. | [optional] 

### Return type

[**[]Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RecommendSimilar**
> []Item RecommendSimilar($storeid, $userid, $itemid, $count)



Return list of recommended items


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **userid** | **string**| User requesting the recommendation | 
 **itemid** | **string**| Similar items bought by others | 
 **count** | **float64**| Return exactly this amount of suggestions. Maximum value is 50, default is 5. | [optional] 

### Return type

[**[]Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RegisterEvent**
> Event RegisterEvent($storeid, $event)



Register new event


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **event** | [**Event**](Event.md)| Single event to register | 

### Return type

[**Event**](Event.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RegisterItem**
> Item RegisterItem($storeid, $item)



Register new item


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 
 **item** | [**Item**](Item.md)| Single item to register | 

### Return type

[**Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RegisterStore**
> Store RegisterStore($store)



Register new Store


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **store** | [**Store**](Store.md)| Store | 

### Return type

[**Store**](Store.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RetrieveEvents**
> []Event RetrieveEvents($storeid)



Get recent events


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 

### Return type

[**[]Event**](Event.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RetrieveItems**
> []Item RetrieveItems($storeid)



Get recent items


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **storeid** | **string**| Store identifier | 

### Return type

[**[]Item**](Item.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

