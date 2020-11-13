### 安装
go get
### 使用
```
func init() {
	logger.SetLogInfo(logger.LOG_LEVEL_DEBUG, logger.LOG_TYPE_STDOUT|logger.LOG_TYPE_FILE, "logs/test.log")
}

func main() {
	logger.LOGD("11")
	logger.SyncToFile()
}
```
