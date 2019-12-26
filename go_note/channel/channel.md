

# channel

go的channel用于多个gorotine传递数据, 是 **Don't communicat by sharing memory; share memory by communicationg**  的体现. 

## channel的使用

### 代码示例

```go
ch1 := make(chan int, 1)
go func() {
   ch1 <- 1
}()
i := <-ch1
```

通过`make`函数创建,在关键字`chan` 后面指定channel能发送的数据类型,  后面的数组表示**缓冲区**的大小.  

###  使用中需要注意的问题

**缓冲区:**  



## channel 的实现









