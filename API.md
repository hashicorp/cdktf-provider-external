# API Reference

**Classes**

Name|Description
----|-----------
[DataExternal](#cdktf-provider-external-dataexternal)|Represents a {@link https://www.terraform.io/docs/providers/external/d/external external}.
[ExternalProvider](#cdktf-provider-external-externalprovider)|Represents a {@link https://www.terraform.io/docs/providers/external external}.


**Structs**

Name|Description
----|-----------
[DataExternalConfig](#cdktf-provider-external-dataexternalconfig)|*No description*
[ExternalProviderConfig](#cdktf-provider-external-externalproviderconfig)|*No description*



## class DataExternal  <a id="cdktf-provider-external-dataexternal"></a>

Represents a {@link https://www.terraform.io/docs/providers/external/d/external external}.

__Implements__: [IConstruct](#constructs-iconstruct), [IDependable](#constructs-idependable), [ITerraformResource](#cdktf-iterraformresource), [ITerraformDependable](#cdktf-iterraformdependable), [ITerraformAddressable](#cdktf-iterraformaddressable), [IInterpolatingParent](#cdktf-iinterpolatingparent)
__Extends__: [TerraformDataSource](#cdktf-terraformdatasource)

### Initializer


Create a new {@link https://www.terraform.io/docs/providers/external/d/external external} Data Source.

```ts
new DataExternal(scope: Construct, id: string, config: DataExternalConfig)
```

* **scope** (<code>[Construct](#constructs-construct)</code>)  The scope in which to define this construct.
* **id** (<code>string</code>)  The scoped construct ID.
* **config** (<code>[DataExternalConfig](#cdktf-provider-external-dataexternalconfig)</code>)  *No description*
  * **connection** (<code>[ISSHProvisionerConnection](#cdktf-isshprovisionerconnection) &#124; [IWinrmProvisionerConnection](#cdktf-iwinrmprovisionerconnection)</code>)  *No description* __*Optional*__
  * **count** (<code>number</code>)  *No description* __*Optional*__
  * **dependsOn** (<code>Array<[ITerraformDependable](#cdktf-iterraformdependable)></code>)  *No description* __*Optional*__
  * **forEach** (<code>[ITerraformIterator](#cdktf-iterraformiterator)</code>)  *No description* __*Optional*__
  * **lifecycle** (<code>[TerraformResourceLifecycle](#cdktf-terraformresourcelifecycle)</code>)  *No description* __*Optional*__
  * **provider** (<code>[TerraformProvider](#cdktf-terraformprovider)</code>)  *No description* __*Optional*__
  * **provisioners** (<code>Array<[IFileProvisioner](#cdktf-ifileprovisioner) &#124; [ILocalExecProvisioner](#cdktf-ilocalexecprovisioner) &#124; [IRemoteExecProvisioner](#cdktf-iremoteexecprovisioner)></code>)  *No description* __*Optional*__
  * **program** (<code>Array<string></code>)  A list of strings, whose first element is the program to run and whose subsequent elements are optional command line arguments to the program. 
  * **id** (<code>string</code>)  Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#id DataExternal#id}. __*Optional*__
  * **query** (<code>Map<string, string></code>)  A map of string values to pass to the external program as the query arguments. __*Optional*__
  * **workingDir** (<code>string</code>)  Working directory of the program. If not supplied, the program will run in the current directory. __*Optional*__



### Properties


Name | Type | Description 
-----|------|-------------
**id** | <code>string</code> | <span></span>
**program** | <code>Array<string></code> | <span></span>
**query** | <code>Map<string, string></code> | <span></span>
**result** | <code>[StringMap](#cdktf-stringmap)</code> | <span></span>
**workingDir** | <code>string</code> | <span></span>
**idInput**? | <code>string</code> | __*Optional*__
**programInput**? | <code>Array<string></code> | __*Optional*__
**queryInput**? | <code>Map<string, string></code> | __*Optional*__
**workingDirInput**? | <code>string</code> | __*Optional*__
*static* **tfResourceType** | <code>string</code> | <span></span>

### Methods


#### resetId() <a id="cdktf-provider-external-dataexternal-resetid"></a>



```ts
resetId(): void
```





#### resetQuery() <a id="cdktf-provider-external-dataexternal-resetquery"></a>



```ts
resetQuery(): void
```





#### resetWorkingDir() <a id="cdktf-provider-external-dataexternal-resetworkingdir"></a>



```ts
resetWorkingDir(): void
```





#### protected synthesizeAttributes() <a id="cdktf-provider-external-dataexternal-synthesizeattributes"></a>



```ts
protected synthesizeAttributes(): Map<string, any>
```


__Returns__:
* <code>Map<string, any></code>



## class ExternalProvider  <a id="cdktf-provider-external-externalprovider"></a>

Represents a {@link https://www.terraform.io/docs/providers/external external}.

__Implements__: [IConstruct](#constructs-iconstruct), [IDependable](#constructs-idependable)
__Extends__: [TerraformProvider](#cdktf-terraformprovider)

### Initializer


Create a new {@link https://www.terraform.io/docs/providers/external external} Resource.

```ts
new ExternalProvider(scope: Construct, id: string, config?: ExternalProviderConfig)
```

* **scope** (<code>[Construct](#constructs-construct)</code>)  The scope in which to define this construct.
* **id** (<code>string</code>)  The scoped construct ID.
* **config** (<code>[ExternalProviderConfig](#cdktf-provider-external-externalproviderconfig)</code>)  *No description*
  * **alias** (<code>string</code>)  Alias name. __*Optional*__



### Properties


Name | Type | Description 
-----|------|-------------
**alias**? | <code>string</code> | __*Optional*__
**aliasInput**? | <code>string</code> | __*Optional*__
*static* **tfResourceType** | <code>string</code> | <span></span>

### Methods


#### resetAlias() <a id="cdktf-provider-external-externalprovider-resetalias"></a>



```ts
resetAlias(): void
```





#### protected synthesizeAttributes() <a id="cdktf-provider-external-externalprovider-synthesizeattributes"></a>



```ts
protected synthesizeAttributes(): Map<string, any>
```


__Returns__:
* <code>Map<string, any></code>



## struct DataExternalConfig  <a id="cdktf-provider-external-dataexternalconfig"></a>






Name | Type | Description 
-----|------|-------------
**program** | <code>Array<string></code> | A list of strings, whose first element is the program to run and whose subsequent elements are optional command line arguments to the program.
**connection**????? | <code>[ISSHProvisionerConnection](#cdktf-isshprovisionerconnection) &#124; [IWinrmProvisionerConnection](#cdktf-iwinrmprovisionerconnection)</code> | __*Optional*__
**count**????? | <code>number</code> | __*Optional*__
**dependsOn**????? | <code>Array<[ITerraformDependable](#cdktf-iterraformdependable)></code> | __*Optional*__
**forEach**????? | <code>[ITerraformIterator](#cdktf-iterraformiterator)</code> | __*Optional*__
**id**? | <code>string</code> | Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#id DataExternal#id}.<br/>__*Optional*__
**lifecycle**????? | <code>[TerraformResourceLifecycle](#cdktf-terraformresourcelifecycle)</code> | __*Optional*__
**provider**????? | <code>[TerraformProvider](#cdktf-terraformprovider)</code> | __*Optional*__
**provisioners**????? | <code>Array<[IFileProvisioner](#cdktf-ifileprovisioner) &#124; [ILocalExecProvisioner](#cdktf-ilocalexecprovisioner) &#124; [IRemoteExecProvisioner](#cdktf-iremoteexecprovisioner)></code> | __*Optional*__
**query**? | <code>Map<string, string></code> | A map of string values to pass to the external program as the query arguments.<br/>__*Optional*__
**workingDir**? | <code>string</code> | Working directory of the program. If not supplied, the program will run in the current directory.<br/>__*Optional*__



## struct ExternalProviderConfig  <a id="cdktf-provider-external-externalproviderconfig"></a>






Name | Type | Description 
-----|------|-------------
**alias**? | <code>string</code> | Alias name.<br/>__*Optional*__



