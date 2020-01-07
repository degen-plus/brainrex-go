# \IntegrationsApi

All URIs are relative to *https://api.bitlongs.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CryptoGetCandleData**](IntegrationsApi.md#CryptoGetCandleData) | **Post** /crypto/get_candles | Downloads candle format market data
[**CryptoGetExchangeAssets**](IntegrationsApi.md#CryptoGetExchangeAssets) | **Post** /crypto/get_exchange_assets | Gets all coin pairs traded in specified exchange
[**CryptoGetOrderbooks**](IntegrationsApi.md#CryptoGetOrderbooks) | **Post** /crypto/get_orderbooks | Returns the current state of the orderbook.
[**CryptoGetSupportedExchanges**](IntegrationsApi.md#CryptoGetSupportedExchanges) | **Get** /crypto/get_supported_exchanges | Gets all cryptocurrency exchanges supported by the Brainrex API
[**CryptoGetTicker**](IntegrationsApi.md#CryptoGetTicker) | **Post** /crypto/get_ticker | Downloads candle format market data


# **CryptoGetCandleData**
> CandleResponse CryptoGetCandleData(ctx, candleRequest)
Downloads candle format market data

Returns a list of candle data from specified market and data range

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **candleRequest** | [**CandleRequest**](CandleRequest.md)| The Get candles end point return market data in Open High Close Volume format. In order to use this endpoint you need to enter your API keys to your data provider in the console | 

### Return type

[**CandleResponse**](CandleResponse.md)

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CryptoGetExchangeAssets**
> ExchangeAssetsResponse CryptoGetExchangeAssets(ctx, exchange)
Gets all coin pairs traded in specified exchange

This endpoint returns all the Available currency pairs

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **exchange** | [**Exchange**](Exchange.md)| Name of the cryptocurrency exchange | 

### Return type

[**ExchangeAssetsResponse**](ExchangeAssetsResponse.md)

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CryptoGetOrderbooks**
> OrderbookResponse CryptoGetOrderbooks(ctx, orderbookRequest)
Returns the current state of the orderbook.

This endpoint returns the current state of the ordebook with a limit set by you. The maximun orderbook depth is 25.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **orderbookRequest** | [**OrderbookRequest**](OrderbookRequest.md)| Exchange, trading pair and date rage for data | 

### Return type

[**OrderbookResponse**](OrderbookResponse.md)

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CryptoGetSupportedExchanges**
> SupportedExchanges CryptoGetSupportedExchanges(ctx, )
Gets all cryptocurrency exchanges supported by the Brainrex API

Returns a list of candle data from specified market and data range

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**SupportedExchanges**](SupportedExchanges.md)

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CryptoGetTicker**
> TickerResponse CryptoGetTicker(ctx, exchange)
Downloads candle format market data

Returns a list of candle data from specified market and data range

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **exchange** | [**Exchange**](Exchange.md)| Get ticker data from specified crypto exchange | 

### Return type

[**TickerResponse**](TickerResponse.md)

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

