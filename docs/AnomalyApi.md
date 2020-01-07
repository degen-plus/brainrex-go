# \AnomalyApi

All URIs are relative to *https://api.bitlongs.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AnomalyBatch**](AnomalyApi.md#AnomalyBatch) | **Post** /anomaly/json/detect | Detects anomalies in historical data in batches. This endpoint uses your entire dataset as input


# **AnomalyBatch**
> []bool AnomalyBatch(ctx, optional)
Detects anomalies in historical data in batches. This endpoint uses your entire dataset as input

The Anomaly Detect endpoint ingests time series data of all types, then monitors and detects abnormalities historical time series data. <br><br> Our AI selects from several models, choosing the one that fits the given data best, and we give you the avality to customize the sensitivy of the model. Our model has been trained to recognize anomalies in popular blockchain networks e.g. Bitcoin, Ethereum, learning from past events.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***AnomalyBatchOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AnomalyBatchOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **request** | [**optional.Interface of TimeSeries**](TimeSeries.md)| Time Series to be analyzed, with the following format. | 

### Return type

**[]bool**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

