Proj_3 Capacity Loss Measurement
=======================

### Usage 使用方式

 1. 打開 `CMD` 或者是 終端機
 2. `cd` 進入本資料夾
 3. Windows: 執行 `EXE` 檔：`capacity_loss_measure.exe` / OSX: 執行 `out` 檔：`capacity_loss_measure.out`
 4. 執行後程式會詢問要輸入的 `n` 值，輸入 `n` 值之後便開始計算 `MXC`

例如：

```
Please input n:2
Calculating ...
 n   | K   | L   | max_k | max     | result
 2   | 1   | 2   | 1     | 262144  | 262144
 2   | 2   | 4   | 1     | 262144  | 262144
 2   | 3   | 6   | 1     | 262144  | 262140
 2   | 4   | 9   | 4     | 294912  | 294912
 2   | 5   | 11  | 4     | 294912  | 288354
 2   | 6   | 13  | 4     | 294912  | 283985
 2   | 7   | 16  | 7     | 299584  | 299584
 2   | 8   | 18  | 7     | 299584  | 294912
 2   | 9   | 20  | 7     | 299584  | 291260
 2   | 10  | 23  | 10    | 301461  | 301461
 2   | 11  | 25  | 10    | 301461  | 297875
 2   | 12  | 27  | 10    | 301461  | 294894
 2   | 13  | 30  | 13    | 302460  | 302460
 2   | 14  | 32  | 13    | 302460  | 299584
 2   | 15  | 34  | 13    | 302460  | 297092
 2   | 16  | 37  | 16    | 303104  | 303104
 2   | 17  | 39  | 16    | 303104  | 300690
 2   | 18  | 41  | 16    | 303104  | 298521
 2   | 19  | 44  | 19    | 303512  | 303512
 2   | 20  | 46  | 19    | 303512  | 301438
 2   | 21  | 48  | 19    | 303512  | 299568
 2   | 22  | 51  | 22    | 303807  | 303807
 2   | 23  | 53  | 22    | 303807  | 301994
 2   | 24  | 55  | 22    | 303807  | 300355
 2   | 25  | 58  | 25    | 304036  | 304036
 2   | 26  | 60  | 25    | 304036  | 302460
 2   | 27  | 62  | 25    | 304036  | 300948
MXC is 304036, max_k: 25, max_L: 58, OPT: 304339.759253, CL: 0.099809 %
```

### 編譯執行

本作業使用 [Go](https://golang.org) 語言開發，`Go` 是 Google 開發的一種編譯型，並發型，並具有垃圾回收功能的程式語言。要編譯必須要先安裝好 `Go` 編譯器，從官網下載安裝完畢之後在 `CMD` 或者終端機輸入下方指令即可編譯：

```
go build
```

下方指令可編譯並執行：

```
go run capacity_loss_measure.go
```