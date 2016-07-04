# WWW::SwaggerClient::DefaultApi

## Load the API package
```perl
use WWW::SwaggerClient::Object::DefaultApi;
```

All URIs are relative to *https://api.pbxdom.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calls_get**](DefaultApi.md#calls_get) | **GET** /Calls | 
[**features_charts_get**](DefaultApi.md#features_charts_get) | **GET** /Features/charts | 
[**features_reports_get**](DefaultApi.md#features_reports_get) | **GET** /Features/reports | 
[**features_widget_get**](DefaultApi.md#features_widget_get) | **GET** /Features/widget | 


# **calls_get**
> ARRAY[InlineResponse200] calls_get(rpt_type => $rpt_type, rpt_id => $rpt_id, start => $start, limit => $limit, sort_by => $sort_by, sort_type => $sort_type, from_date => $from_date, to_date => $to_date, duration => $duration, phone => $phone, phone1 => $phone1, co => $co, ext => $ext, pbx_id => $pbx_id, call_source => $call_source, call_type => $call_type, direction => $direction, caller_name => $caller_name, did => $did, dnis => $dnis, acc => $acc, ring => $ring, cost => $cost, group => $group)



Gets `Calls` info. 

### Example 
```perl
use Data::Dumper;

my $api_instance = WWW::SwaggerClient::DefaultApi->new();
my $rpt_type = 1.2; # double | Report type. (0 report, 1 widget, 2 chart).
my $rpt_id = 1.2; # double | Report id.
my $start = 3.4; # Number | Start offset.
my $limit = 3.4; # Number | Number of results to return. Max 10K.
my $sort_by = 'sort_by_example'; # string | Sort column.
my $sort_type = 'sort_type_example'; # string | Sort mode asc/desc.
my $from_date = 'from_date_example'; # string | Start date time.
my $to_date = 'to_date_example'; # string | End date time.
my $duration = 3.4; # Number | Duration range.
my $phone = 'phone_example'; # string | List of caller phone.
my $phone1 = 'phone1_example'; # string | List of dialled phones.
my $co = 'co_example'; # string | List of trunk/co.
my $ext = 'ext_example'; # string | list of extensions.
my $pbx_id = 3.4; # Number | list of PBX Ids.
my $call_source = 3.4; # Number | list of callsource.
my $call_type = 3.4; # Number | list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls)
my $direction = 3.4; # Number | list of direction.(0 incoming, 1 outgoing, 2 internal)
my $caller_name = 'caller_name_example'; # string | list of caller name.
my $did = 'did_example'; # string | list of did.
my $dnis = 'dnis_example'; # string | list of dnis.
my $acc = 'acc_example'; # string | list of account code.
my $ring = 3.4; # Number | Ring range.Seconds unit.
my $cost = 3.4; # Number | Cost range.
my $group = 3.4; # Number | Department/Group id.

eval { 
    my $result = $api_instance->calls_get(rpt_type => $rpt_type, rpt_id => $rpt_id, start => $start, limit => $limit, sort_by => $sort_by, sort_type => $sort_type, from_date => $from_date, to_date => $to_date, duration => $duration, phone => $phone, phone1 => $phone1, co => $co, ext => $ext, pbx_id => $pbx_id, call_source => $call_source, call_type => $call_type, direction => $direction, caller_name => $caller_name, did => $did, dnis => $dnis, acc => $acc, ring => $ring, cost => $cost, group => $group);
    print Dumper($result);
};
if ($@) {
    warn "Exception when calling DefaultApi->calls_get: $@\n";
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rpt_type** | **double**| Report type. (0 report, 1 widget, 2 chart). | 
 **rpt_id** | **double**| Report id. | 
 **start** | **Number**| Start offset. | [optional] 
 **limit** | **Number**| Number of results to return. Max 10K. | [optional] 
 **sort_by** | **string**| Sort column. | [optional] 
 **sort_type** | **string**| Sort mode asc/desc. | [optional] 
 **from_date** | **string**| Start date time. | [optional] 
 **to_date** | **string**| End date time. | [optional] 
 **duration** | **Number**| Duration range. | [optional] 
 **phone** | **string**| List of caller phone. | [optional] 
 **phone1** | **string**| List of dialled phones. | [optional] 
 **co** | **string**| List of trunk/co. | [optional] 
 **ext** | **string**| list of extensions. | [optional] 
 **pbx_id** | **Number**| list of PBX Ids. | [optional] 
 **call_source** | **Number**| list of callsource. | [optional] 
 **call_type** | **Number**| list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls) | [optional] 
 **direction** | **Number**| list of direction.(0 incoming, 1 outgoing, 2 internal) | [optional] 
 **caller_name** | **string**| list of caller name. | [optional] 
 **did** | **string**| list of did. | [optional] 
 **dnis** | **string**| list of dnis. | [optional] 
 **acc** | **string**| list of account code. | [optional] 
 **ring** | **Number**| Ring range.Seconds unit. | [optional] 
 **cost** | **Number**| Cost range. | [optional] 
 **group** | **Number**| Department/Group id. | [optional] 

### Return type

[**ARRAY[InlineResponse200]**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **features_charts_get**
> ARRAY[InlineResponse200] features_charts_get()



Gets `Charts` list. 

### Example 
```perl
use Data::Dumper;

my $api_instance = WWW::SwaggerClient::DefaultApi->new();

eval { 
    my $result = $api_instance->features_charts_get();
    print Dumper($result);
};
if ($@) {
    warn "Exception when calling DefaultApi->features_charts_get: $@\n";
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ARRAY[InlineResponse200]**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **features_reports_get**
> ARRAY[InlineResponse200] features_reports_get()



Gets `Reports` list. 

### Example 
```perl
use Data::Dumper;

my $api_instance = WWW::SwaggerClient::DefaultApi->new();

eval { 
    my $result = $api_instance->features_reports_get();
    print Dumper($result);
};
if ($@) {
    warn "Exception when calling DefaultApi->features_reports_get: $@\n";
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ARRAY[InlineResponse200]**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **features_widget_get**
> ARRAY[InlineResponse200] features_widget_get()



Gets `Widgets` list. 

### Example 
```perl
use Data::Dumper;

my $api_instance = WWW::SwaggerClient::DefaultApi->new();

eval { 
    my $result = $api_instance->features_widget_get();
    print Dumper($result);
};
if ($@) {
    warn "Exception when calling DefaultApi->features_widget_get: $@\n";
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ARRAY[InlineResponse200]**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

