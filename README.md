Go-WeiboSDK
===========

Sina weibo api in golang
-----------

## Example

```go
	wb := weibo.New("APPKey", "APPSecret")
	userTimeline, errChan := wb.Statuses.UserTimeline(access_token, uid, "", options) // options is of type map[string]interface{}
	if err:=<-errChan; err!=nil {
		panic(err)
	}
	fmt.Println(userTimeline.Statuses)
```
