# 删除AI图片信息

调用DeleteAIImageInfos删除AI图片信息。

**说明：** 此接口只是删除AI图片信息，并不会实际删除图片文件。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=vod&api=DeleteAIImageInfos&type=RPC&version=2017-03-21)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DeleteAIImageInfos|系统规定参数，取值：**DeleteAIImageInfos** |
|AIImageInfoIds|String|是|b89a6aabf144\*\*\*\*\*6197ebd6fe6cf29|AI图片文件ID，英文逗号分隔，最大支持10个ID。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|FCDC80EA-363C-41\*\*\*\*\*B8-0DF14033D643|请求ID。 |

**说明：** 下述请求示例中的“公共请求参数”详情，参见[公共参数说明文档](~~44432~~)。

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=DeleteAIImageInfos
&AIImageInfoIds=b89a6aabf144*****6197ebd6fe6cf29
&<公共请求参数>
```

正常返回示例

`XML` 格式

```
<DeleteAIImageInfosResponse>
      <RequestId>FCDC80EA-363C-41*****B8-0DF14033D643</RequestId>
</DeleteAIImageInfosResponse>
```

`JSON` 格式

```
{
    "RequestId":"FCDC80EA-363C-41*****B8-0DF14033D643"
}
```

## 错误码

访问[错误中心](https://error-center.aliyun.com/status/product/vod)查看更多错误码。

