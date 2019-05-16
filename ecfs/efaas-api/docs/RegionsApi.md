# \RegionsApi

All URIs are relative to *https://localhost/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListRegions**](RegionsApi.md#ListRegions) | **Get** /regions | Retrieves the list of region resources available for service


# **ListRegions**
> []Region ListRegions($filter)

Retrieves the list of region resources available for service


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **string**| A filter expression that filters resources listed in the response. The expression must specify the field name, a comparison operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The comparison operator must be either &#x3D;, !&#x3D;, &gt;, or &lt;.  For example, if you are filtering Service Class you can include only Service Classes with node type equal to medium by specifying nodeType &#x3D; medium.  To filter nested fields use regions.name &#x3D; us-central1 to include Service Class available in us-central1 region.  To filter on multiple expressions, provide each separate expression within parentheses. For example, (regions.name &#x3D; us-central1) (nodeType &#x3D; medium) | [optional] 

### Return type

[**[]Region**](region.md)

### Authorization

[cloud-console-partner](../README.md#cloud-console-partner), [cloud-console-partner-autopush](../README.md#cloud-console-partner-autopush), [google-id](../README.md#google-id), [cloud-console-partner-local](../README.md#cloud-console-partner-local)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
