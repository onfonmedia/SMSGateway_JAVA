# Getting started

Send SMS with Onfon Media SMS Platform.

## How to Build

The generated code uses a few Maven dependencies e.g., Jackson, UniRest,
and Apache HttpClient. The reference to these dependencies is already
added in the pom.xml file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Eclipse click on ``` File -> Import ```.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/java?step=import0&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

* In the import dialog, select ``` Existing Java Project ``` and click ``` Next ```.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/java?step=import1&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

* Browse to locate the folder containing the source code. Select the detected location of the project and click ``` Finish ```.

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/java?step=import2&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

* Upon successful import, the project will be automatically built by Eclipse after automatically resolving the dependencies.

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/java?step=import3&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

## How to Use

The following section explains how to use the OnfonMediaSMSGateway library in a new console project.

### 1. Starting a new project

For starting a new project, click the menu command ``` File > New > Project ```.

![Add a new project in Eclipse](https://apidocs.io/illustration/java?step=createNewProject0&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

Next, choose ``` Maven > Maven Project ```and click ``` Next ```.

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/java?step=createNewProject1&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

Here, make sure to use the current workspace by choosing ``` Use default Workspace location ```, as shown in the picture below and click ``` Next ```.

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/java?step=createNewProject2&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

Following this, select the *quick start* project type to create a simple project with an existing class and a ``` main ``` method. To do this, choose ``` maven-archetype-quickstart ``` item from the list and click ``` Next ```.

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/java?step=createNewProject3&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

In the last step, provide a ``` Group Id ``` and ``` Artifact Id ``` as shown in the picture below and click ``` Finish ```.

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/java?step=createNewProject4&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

### 2. Add reference of the library project

The created Maven project manages its dependencies using its ``` pom.xml ``` file. In order to add a dependency on the *OnfonMediaSMSGatewayLib* client library, double click on the ``` pom.xml ``` file in the ``` Package Explorer ```. Opening the ``` pom.xml ``` file will render a graphical view on the cavas. Here, switch to the ``` Dependencies ``` tab and click the ``` Add ``` button as shown in the picture below.

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/java?step=testProject0&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

Clicking the ``` Add ``` button will open a dialog where you need to specify OnfonMediaSMSGateway in ``` Group Id ``` and OnfonMediaSMSGatewayLib in the ``` Artifact Id ``` fields. Once added click ``` OK ```. Save the ``` pom.xml ``` file.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject1&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

### 3. Write sample code

Once the ``` SimpleConsoleApp ``` is created, a file named ``` App.java ``` will be visible in the *Package Explorer* with a ``` main ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject2&workspaceFolder=OnfonMedia%20SMS%20Gateway-Java&workspaceName=OnfonMediaSMSGateway&projectName=OnfonMediaSMSGatewayLib&rootNamespace=ke.co.onfonmedia.api)

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project *OnfonMediaSMSGatewayLib* from the package explorer.
2. Select "Run -> Run as -> JUnit Test" or use "Alt + Shift + X" followed by "T" to run the Tests.

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| accessKey | Network Layer Access Key |
| apiKey | Used for authentication purpose and pass this parameter in URL encoded format. |
| clientId | Used for authentication purpose and pass this parameter in URL encoded format. |



API client can be initialized as following.

```java
// Configuration parameters and credentials
String accessKey = "ACCESS_KEY"; // Network Layer Access Key
String apiKey = "API_KEY"; // Used for authentication purpose and pass this parameter in URL encoded format.
String clientId = "CLIENT_ID"; // Used for authentication purpose and pass this parameter in URL encoded format.

OnfonMediaSMSGatewayClient client = new OnfonMediaSMSGatewayClient(accessKey, apiKey, clientId);
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AccountController](#account_controller)
* [TemplateController](#template_controller)
* [SMSController](#sms_controller)
* [GROUPController](#group_controller)
* [CampaignController](#campaign_controller)

## <a name="account_controller"></a>![Class: ](https://apidocs.io/img/class.png "ke.co.onfonmedia.api.controllers.AccountController") AccountController

### Get singleton instance

The singleton instance of the ``` AccountController ``` class can be accessed from the API Client.

```java
AccountController account = client.getAccount();
```

### <a name="get_credit_balance_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.AccountController.getCreditBalanceAsync") getCreditBalanceAsync

> Get Credit Balance


```java
void getCreditBalanceAsync(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
account.getCreditBalanceAsync(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="template_controller"></a>![Class: ](https://apidocs.io/img/class.png "ke.co.onfonmedia.api.controllers.TemplateController") TemplateController

### Get singleton instance

The singleton instance of the ``` TemplateController ``` class can be accessed from the API Client.

```java
TemplateController template = client.getTemplate();
```

### <a name="get_template_list_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.TemplateController.getTemplateListAsync") getTemplateListAsync

> Get Template List


```java
void getTemplateListAsync(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
template.getTemplateListAsync(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_new_template_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.TemplateController.createNewTemplateAsync") createNewTemplateAsync

> Create New Template


```java
void createNewTemplateAsync(
        final String messageTemplate,
        final String templateName,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageTemplate |  ``` Required ```  | Template text. |
| templateName |  ``` Required ```  | Name of template |


#### Example Usage

```java
String messageTemplate = "MessageTemplate";
String templateName = "TemplateName";
// Invoking the API call with sample inputs
template.createNewTemplateAsync(messageTemplate, templateName, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_template_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.TemplateController.updateTemplateAsync") updateTemplateAsync

> Update Template


```java
void updateTemplateAsync(
        final String messageTemplate,
        final String templateName,
        final int id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageTemplate |  ``` Required ```  | Template text. |
| templateName |  ``` Required ```  | Name of template |
| id |  ``` Required ```  | id of template |


#### Example Usage

```java
String messageTemplate = "MessageTemplate";
String templateName = "TemplateName";
int id = 208;
// Invoking the API call with sample inputs
template.updateTemplateAsync(messageTemplate, templateName, id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="delete_template_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.TemplateController.deleteTemplateAsync") deleteTemplateAsync

> Delete Template


```java
void deleteTemplateAsync(
        final int id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id of template |


#### Example Usage

```java
int id = 208;
// Invoking the API call with sample inputs
template.deleteTemplateAsync(id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png "ke.co.onfonmedia.api.controllers.SMSController") SMSController

### Get singleton instance

The singleton instance of the ``` SMSController ``` class can be accessed from the API Client.

```java
SMSController sMS = client.getSMS();
```

### <a name="get_sent_message_list_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.SMSController.getSentMessageListAsync") getSentMessageListAsync

> Get Sent Message List


```java
void getSentMessageListAsync(
        final LocalDate enddate,
        final LocalDate fromdate,
        final int length,
        final int start,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| enddate |  ``` Required ```  | Date format must be in yyyy-mm-dd |
| fromdate |  ``` Required ```  | Date format must be in yyyy-mm-dd |
| length |  ``` Required ```  | Ending index value to fetch the campaign detail. |
| start |  ``` Required ```  | Starting index value to fetch the campaign detail. |


#### Example Usage

```java
LocalDate enddate = new Date();
LocalDate fromdate = new Date();
int length = 208;
int start = 208;
// Invoking the API call with sample inputs
sMS.getSentMessageListAsync(enddate, fromdate, length, start, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_sent_message_status_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.SMSController.getSentMessageStatusAsync") getSentMessageStatusAsync

> Get Sent Message Status


```java
void getSentMessageStatusAsync(
        final int messageId,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | MessageId of message |


#### Example Usage

```java
int messageId = 208;
// Invoking the API call with sample inputs
sMS.getSentMessageStatusAsync(messageId, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_create_sms_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.SMSController.getCreateSMSAsync") getCreateSMSAsync

> Create SMS


```java
void getCreateSMSAsync(
        final String message,
        final String mobileNumber,
        final String senderId,
        final String coRelator,
        final Boolean isFlash,
        final Boolean isUnicode,
        final String linkId,
        final String groupId,
        final String scheduleTime,
        final String serviceId,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| message |  ``` Required ```  | text message to send |
| mobileNumber |  ``` Required ```  | Use mobile number as comma sepreated to send message on multiple mobile number e.g. 78461230,78945612 |
| senderId |  ``` Required ```  | Approved Sender Id |
| coRelator |  ``` Optional ```  | Parameter required for using SDP OnDemand Service |
| isFlash |  ``` Optional ```  | Is_Flash is true or false for flash message |
| isUnicode |  ``` Optional ```  | Is_Unicode is true or false for unicode message |
| linkId |  ``` Optional ```  | Parameter required for using SDP OnDemand Service |
| groupId |  ``` Optional ```  | Valid group-id of current user (only for group message otherwise leave empty string) |
| scheduleTime |  ``` Optional ```  | scheduleTime Date in yyyy-MM-dd HH:MM (only for schedule message) |
| serviceId |  ``` Optional ```  | Parameter required for using SDP OnSubscription Service |


#### Example Usage

```java
String message = "Message";
String mobileNumber = "MobileNumber";
String senderId = "SenderId";
String coRelator = "CoRelator";
Boolean isFlash = true;
Boolean isUnicode = true;
String linkId = "LinkId";
String groupId = "groupId";
String scheduleTime = "scheduleTime";
String serviceId = "serviceId";
// Invoking the API call with sample inputs
sMS.getCreateSMSAsync(message, mobileNumber, senderId, coRelator, isFlash, isUnicode, linkId, groupId, scheduleTime, serviceId, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_sms_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.SMSController.createSMSAsync") createSMSAsync

> Create SMS


```java
void createSMSAsync(
        final String message,
        final String mobileNumber,
        final String senderId,
        final String coRelator,
        final Boolean isFlash,
        final Boolean isUnicode,
        final String linkId,
        final String groupId,
        final String scheduleTime,
        final String serviceId,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| message |  ``` Required ```  | text message to send |
| mobileNumber |  ``` Required ```  | Use mobile number as comma sepreated to send message on multiple mobile number e.g. 78461230,78945612 |
| senderId |  ``` Required ```  | Approved Sender Id |
| coRelator |  ``` Optional ```  | Parameter required for using SDP OnDemand Service |
| isFlash |  ``` Optional ```  | Is_Flash is true or false for flash message |
| isUnicode |  ``` Optional ```  | Is_Unicode is true or false for unicode message |
| linkId |  ``` Optional ```  | Parameter required for using SDP OnDemand Service |
| groupId |  ``` Optional ```  | Valid group-id of current user (only for group message otherwise leave empty string) |
| scheduleTime |  ``` Optional ```  | scheduleTime Date in yyyy-MM-dd HH:MM (only for schedule message) |
| serviceId |  ``` Optional ```  | Parameter required for using SDP OnSubscription Service |


#### Example Usage

```java
String message = "Message";
String mobileNumber = "MobileNumber";
String senderId = "SenderId";
String coRelator = "CoRelator";
Boolean isFlash = true;
Boolean isUnicode = true;
String linkId = "LinkId";
String groupId = "groupId";
String scheduleTime = "scheduleTime";
String serviceId = "serviceId";
// Invoking the API call with sample inputs
sMS.createSMSAsync(message, mobileNumber, senderId, coRelator, isFlash, isUnicode, linkId, groupId, scheduleTime, serviceId, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_create_bulk_sms_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.SMSController.getCreateBulkSMSAsync") getCreateBulkSMSAsync

> Create Bulk SMS


```java
void getCreateBulkSMSAsync(
        final String mobileNumberMessage,
        final String senderId,
        final String coRelator,
        final Boolean isFlash,
        final Boolean isUnicode,
        final String linkId,
        final LocalDate scheduleTime,
        final String serviceId,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mobileNumberMessage |  ``` Required ```  | Please ensure while submitting the request the message should be passed in encoded format. e.g. 78461230^test~78945612^hello |
| senderId |  ``` Required ```  | Approved Sender Id |
| coRelator |  ``` Optional ```  | Parameter required for using SDP OnDemand Service |
| isFlash |  ``` Optional ```  | Is_Flash is true or false for flash message |
| isUnicode |  ``` Optional ```  | Is_Unicode is true or false for unicode message |
| linkId |  ``` Optional ```  | Parameter required for using SDP OnDemand Service |
| scheduleTime |  ``` Optional ```  | scheduleTime Date in yyyy-MM-dd HH:MM (only for schedule message) |
| serviceId |  ``` Optional ```  | Parameter required for using SDP OnSubscription Service |


#### Example Usage

```java
String mobileNumberMessage = "MobileNumber_Message";
String senderId = "SenderId";
String coRelator = "CoRelator";
Boolean isFlash = true;
Boolean isUnicode = true;
String linkId = "LinkId";
LocalDate scheduleTime = new Date();
String serviceId = "serviceId";
// Invoking the API call with sample inputs
sMS.getCreateBulkSMSAsync(mobileNumberMessage, senderId, coRelator, isFlash, isUnicode, linkId, scheduleTime, serviceId, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_bulk_sms_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.SMSController.createBulkSMSAsync") createBulkSMSAsync

> Create Bulk SMS


```java
void createBulkSMSAsync(
        final List<String> messageParameters,
        final String senderId,
        final Boolean isFlash,
        final Boolean isUnicode,
        final LocalDate scheduleDateTime,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageParameters |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| senderId |  ``` Required ```  | Approved Sender Id |
| isFlash |  ``` Optional ```  | Is_Flash is true or false for flash message |
| isUnicode |  ``` Optional ```  | Is_Unicode is true or false for unicode message |
| scheduleDateTime |  ``` Optional ```  | scheduleTime Date in yyyy-MM-dd HH:MM (only for schedule message) |


#### Example Usage

```java
List<String> messageParameters = new LinkedList<String>(Arrays.asList("MessageParameters"));
String senderId = "SenderId";
Boolean isFlash = true;
Boolean isUnicode = true;
LocalDate scheduleDateTime = new Date();
// Invoking the API call with sample inputs
sMS.createBulkSMSAsync(messageParameters, senderId, isFlash, isUnicode, scheduleDateTime, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="group_controller"></a>![Class: ](https://apidocs.io/img/class.png "ke.co.onfonmedia.api.controllers.GROUPController") GROUPController

### Get singleton instance

The singleton instance of the ``` GROUPController ``` class can be accessed from the API Client.

```java
GROUPController gROUP = client.getGROUP();
```

### <a name="get_group_list_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.GROUPController.getGroupListAsync") getGroupListAsync

> Get Group List


```java
void getGroupListAsync(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
gROUP.getGroupListAsync(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_new_group_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.GROUPController.createNewGroupAsync") createNewGroupAsync

> Create New Group


```java
void createNewGroupAsync(
        final String groupName,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| groupName |  ``` Required ```  | Name for new group |


#### Example Usage

```java
String groupName = "GroupName";
// Invoking the API call with sample inputs
gROUP.createNewGroupAsync(groupName, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_group_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.GROUPController.updateGroupAsync") updateGroupAsync

> Update Group


```java
void updateGroupAsync(
        final String groupName,
        final String id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| groupName |  ``` Required ```  | Name for new group |
| id |  ``` Required ```  | GroupID |


#### Example Usage

```java
String groupName = "GroupName";
String id = "id";
// Invoking the API call with sample inputs
gROUP.updateGroupAsync(groupName, id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_sub_group_group_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.GROUPController.createSubGroupGroupAsync") createSubGroupGroupAsync

> Create Sub-Group Group


```java
void createSubGroupGroupAsync(
        final String groupName,
        final String id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| groupName |  ``` Required ```  | Name for new group |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String groupName = "GroupName";
String id = "Id";
// Invoking the API call with sample inputs
gROUP.createSubGroupGroupAsync(groupName, id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="delete_group_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.GROUPController.deleteGroupAsync") deleteGroupAsync

> Delete Group


```java
void deleteGroupAsync(
        final int id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
int id = 208;
// Invoking the API call with sample inputs
gROUP.deleteGroupAsync(id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="campaign_controller"></a>![Class: ](https://apidocs.io/img/class.png "ke.co.onfonmedia.api.controllers.CampaignController") CampaignController

### Get singleton instance

The singleton instance of the ``` CampaignController ``` class can be accessed from the API Client.

```java
CampaignController campaign = client.getCampaign();
```

### <a name="get_campaign_message_status_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.CampaignController.getCampaignMessageStatusAsync") getCampaignMessageStatusAsync

> Get Campaign Message Status


```java
void getCampaignMessageStatusAsync(
        final int campaignId,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | First user have to call Get Campaigns api for CampaignId |


#### Example Usage

```java
int campaignId = 208;
// Invoking the API call with sample inputs
campaign.getCampaignMessageStatusAsync(campaignId, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_campaigns_async"></a>![Method: ](https://apidocs.io/img/method.png "ke.co.onfonmedia.api.controllers.CampaignController.getCampaignsAsync") getCampaignsAsync

> Get Campaigns


```java
void getCampaignsAsync(
        final LocalDate enddate,
        final LocalDate fromdate,
        final int length,
        final int start,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| enddate |  ``` Required ```  | Date format must be in yyyy-mm-dd |
| fromdate |  ``` Required ```  | Date format must be in yyyy-mm-dd |
| length |  ``` Required ```  | Ending index value to fetch the campaign detail. |
| start |  ``` Required ```  | Starting index value to fetch the campaign detail. |


#### Example Usage

```java
LocalDate enddate = new Date();
LocalDate fromdate = new Date();
int length = 208;
int start = 208;
// Invoking the API call with sample inputs
campaign.getCampaignsAsync(enddate, fromdate, length, start, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)



