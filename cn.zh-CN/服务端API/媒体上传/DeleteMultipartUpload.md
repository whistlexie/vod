# DeleteMultipartUpload {#doc_api_vod_DeleteMultipartUpload .reference}

调用DeleteMultipartUpload立即删除上传中产生的碎片文件。

**说明：** 文件上传完成后，碎片文件会自动删除；另外点播系统bucket有自动清理机制，过期后碎片文件会自动删除。调用删除视频接口DeleteVideo，会自动触发删除视频碎片文件；调用本接口不会删除视频原始文件和转码后文件。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=vod&api=DeleteMultipartUpload&type=RPC&version=2017-03-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DeleteMultipartUpload|系统规定参数，取值：**DeleteMultipartUpload**。

 |
|MediaId|String|是|1234abcd|媒体ID。

 |
|MediaType|String|是|video|媒体类型，取值：**video（音视频）**。

 |
|AccessKeyId|String|否|your-acceskey-id|访问凭证。

 |
|ResourceRealOwnerId|Long|否|34624557|资源所有者ID。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|25818875-5F78-4A13-BEF6-D7393642CA58|请求ID。

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DeleteMultipartUpload
&MediaId=1234abcd
&MediaType=video
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DeleteMultipartUploadResponse>
	  <RequestId>25818875-5F78-4A13-BEF6-D7393642CA58</RequestId>
</DeleteMultipartUploadResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"RequestId":"25818875-5F78-4A13-BEF6-D7393642CA58"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/vod)查看更多错误码。

