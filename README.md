# robosys_kadai1
## 説明
第7回,第8回で作成したデバイスドライバーをベースに，オリジナリティーある改造をして，LEDを光らせる．
今回は航空機についている赤いランプ（アンチコリジョンライト）と同様の光り方を再現した．
赤いLEDはGPIO25に接続した．
## 使用したもの
- Raspberry Pi 3 Model B+ ×1
- ブレットボード ×1
- LED(赤) ×1
- 抵抗 220Ω ×1
- ジャンパー線 ×3
## 実行手順
```
$ git clone https://github.com/kengo-0805/robosys_kadai1.git
$ cd robosys_kadai1
$ sudo insmod myled.ko
$ sudo chmod 666/dev/mled0
$ echo 0 > /dev/myled0
```

echo 0 > /dev/myled0を実行することによってLEDが10回点滅する．
## 動作の映像
https://youtu.be/abD6gn3JsJg