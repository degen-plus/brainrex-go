# \LanguageApi

All URIs are relative to *https://api.bitlongs.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**LanguageGetCryptoEntities**](LanguageApi.md#LanguageGetCryptoEntities) | **Post** /entity/get_crypto_entities | Extracts known crypto entities like coin names, exchanges, media from text.
[**LanguageGetGeneralSentiment**](LanguageApi.md#LanguageGetGeneralSentiment) | **Post** /sentiment/get_general_sentiment | Returns a -1 to 1 score, depending on positive/negative sentiment
[**LanguageGetPriceSentiment**](LanguageApi.md#LanguageGetPriceSentiment) | **Post** /language/get_price_sentiment | Sentiment analysis score using a model trained for buy signals.


# **LanguageGetCryptoEntities**
> LanguageGetCryptoEntities(ctx, text)
Extracts known crypto entities like coin names, exchanges, media from text.

The Crypto Entities endpoint ingests written MIT Digital Currency Initiative Paper A paper describing how our sentiment and entity analyzer are built. And how the can be used for trading several cryptocurrencies successfully  We prove that using sentiment only as a input to a trading algorithm can be profitable. If combined with other machine learning models. We descri This Paper could be published in MIT Crypto Economics Journal . . <br><br> Our AI selects from several models, choosing the one that fits the given data best, and we give you the avality to customize the sensitivy of the model. Our model has been trained to recognize anomalies in popular blockchain networks e.g. Bitcoin, Ethereum, learning from past events.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **text** | [**Text**](Text.md)| String of text to be analyze for investor sentiment. | 

### Return type

 (empty response body)

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **LanguageGetGeneralSentiment**
> string LanguageGetGeneralSentiment(ctx, text)
Returns a -1 to 1 score, depending on positive/negative sentiment

This endpoints returns a score from -1 to +1 where depending on negative or positive attitude in the text.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **text** | [**Text**](Text.md)| String of text to be analyze for general sentiment. | 

### Return type

**string**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **LanguageGetPriceSentiment**
> string LanguageGetPriceSentiment(ctx, text)
Sentiment analysis score using a model trained for buy signals.

Gives a 0 to 1 score, depending on buy/sell sentiment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **text** | [**Text**](Text.md)| String of text to be analyze for investor sentiment. | 

### Return type

**string**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

