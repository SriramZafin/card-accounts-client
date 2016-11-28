# DefaultApi

All URIs are relative to *https://localhost:8080/localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAccount**](DefaultApi.md#createAccount) | **POST** /accounts | Creates an account
[**deleetAccount**](DefaultApi.md#deleetAccount) | **DELETE** /account-delete/{accountNumber} | Account details delete
[**getAccountDetails**](DefaultApi.md#getAccountDetails) | **GET** /accounts/{accountNumber} | Gets the account details for the given account number
[**getAllAccounts**](DefaultApi.md#getAllAccounts) | **GET** /accounts | Gets account details
[**updateAccountDetails**](DefaultApi.md#updateAccountDetails) | **PUT** /account-update/{accountNumber} | Account details update


<a name="createAccount"></a>
# **createAccount**
> createAccount(accountDetails)

Creates an account

Adds a new account to the Finkit system.

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
AccountDetails accountDetails = new AccountDetails(); // AccountDetails | The account to be created.
try {
    apiInstance.createAccount(accountDetails);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#createAccount");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountDetails** | [**AccountDetails**](AccountDetails.md)| The account to be created. | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="deleetAccount"></a>
# **deleetAccount**
> deleetAccount(accountNumber)

Account details delete

Deletes the account details for the given accountNumber

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Integer accountNumber = 56; // Integer | The person's accountNumber
try {
    apiInstance.deleetAccount(accountNumber);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#deleetAccount");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountNumber** | **Integer**| The person&#39;s accountNumber |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getAccountDetails"></a>
# **getAccountDetails**
> AccountDetails getAccountDetails(accountNumber)

Gets the account details for the given account number

Returns teh account details for the given account number

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Integer accountNumber = 56; // Integer | The person's accountNumber
try {
    AccountDetails result = apiInstance.getAccountDetails(accountNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAccountDetails");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountNumber** | **Integer**| The person&#39;s accountNumber |

### Return type

[**AccountDetails**](AccountDetails.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getAllAccounts"></a>
# **getAllAccounts**
> Accounts getAllAccounts()

Gets account details

Returns a list containing all account details

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    Accounts result = apiInstance.getAllAccounts();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAllAccounts");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Accounts**](Accounts.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="updateAccountDetails"></a>
# **updateAccountDetails**
> updateAccountDetails(accountNumber)

Account details update

Updates the account details for the given accountNumber

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Integer accountNumber = 56; // Integer | The person's accountNumber
try {
    apiInstance.updateAccountDetails(accountNumber);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#updateAccountDetails");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountNumber** | **Integer**| The person&#39;s accountNumber |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

