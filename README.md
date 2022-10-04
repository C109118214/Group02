# Group 2  Communism
***
| Position     | Member             | Work     |
| :----------- | :---------------| :---------- |
| 組長         | C109118214 [朱晉瑭](https://github.com/C109118214) |資料蒐集、資料處理、 內容編整|
| 組長         | C109118226 [林志穎](https://github.com/ZYLinked) |  統整討論資料、影片拍攝、影片剪輯|
| 組長         | C109118227 [謝岷翰](https://github.com/C109118227) |內容編整、問卷製作、發放問卷|
| 組長         | C109118236 [劉　議](https://github.com/C109118236) |統整討論資料、簡報製作|
| 組長         | C109118244 [袁祥竣](https://github.com/C109118244) |程式編寫、程式除錯|
***

### Mermaid
```mermaid
gantt
    title The Schedule of Communism

    section The Beginning of Communism
    Task A      :active,  des1,2022-10-01  , 2022-10-04
    section Communism 2
    Task B      :         des2, after des1 , 10d
    section Communism 3
    Task C      :         des3, after des2  , 10d
    section Communism 4
    Task D      :         des4, after des3  , 10d
```


```graphviz
digraph hierarchy {

                nodesep=1.0 // increases the separation between nodes
                
                node [color=Red,fontname=Courier,shape=box] //All nodes will this shape and colour
                edge [color=Blue, style=dashed] //All the lines look like this

                Headteacher->{Deputy1 Deputy2 BusinessManager}
                Deputy1->{Teacher1 Teacher2}
                BusinessManager->ITManager
                {rank=same;ITManager Teacher1 Teacher2}  // Put them on the same level
}
```
digraph {
	node[shape=record];
	rankdir="LR";
    no1 [label = "研擬計畫 | 編號:1 | 開始:第1天 | 結束:第2天 | 需時:1天"]
    no2 [label = "任務分配 | 編號:2 | 開始:第2天 | 結束:第6天 | 需時:4天"]
    no3 [label = "取得硬體 | 編號:3 | 開始:第2天 | 結束:第19天 | 需時:17天"]
    no4 [label = "程式開發 | 編號:4 | 開始:第6天 | 結束:第76天 | 需時:70天"]
    {rank=same;no3 no2}
    no5 [label = "安裝硬體 | 編號:5 | 開始:第19天 | 結束:第29天 | 需時:10天"]
    no6 [label = "程式測試 | 編號:6 | 開始:第76天 | 結束:第106天 | 需時:30天"]
    no7 [label = "撰寫使用手冊 | 編號:7 | 開始:第29天 | 結束:第54天 | 需時:25天"]
    no8 [label = "轉換檔案 | 編號:8 | 開始:第29天 | 結束:第49天 | 需時:20天"]
    no9 [label = "系統測試 | 編號:9 | 開始:第106天 | 結束:第134天 | 需時:25天"]
    no10 [label = "使用者訓練 | 編號:10 | 開始:第54天 | 結束:第74天 | 需時:20天"]
    no11 [label = "使用者測試 | 編號:11 | 開始:第134天 | 結束:第159天 | 需時:25天"]
    no1->no2
    no1->no3
    no2->no4
    no3->no5
    no4->no6
    no5->no7
    no5->no8
    no6->no9
    no7->no10
    no8->no10
    no9->no11
    no10->no11
    
}
