### 安装
go get -u github.com/wyy8261/go-simplelog
### 使用
```
func init() {
	logger.SetLogInfo(logger.LOG_LEVEL_DEBUG, logger.LOG_TYPE_STDOUT|logger.LOG_TYPE_FILE, "logs/test.log")
}

func main() {
	logger.LOGD("11")
	logger.LOGI("22")
	logger.LOGW("33")
	logger.LOGE("44")
	logger.SyncToFile()
}
```
