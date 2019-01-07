# myled2
ロボットシステム学課題1  
Raspberry Piのデバイスドライバを作りLEDを発光させる。  
GPIO25(22番ピン)を使用する。  
追加機能としてタイマーを実装。

# 実行方法
```bash
$ git clone https://github.com/Kazuma0716/myled2.git
$ cd myled
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
###点灯###
$ echo 1 > /dev/myled0
###消灯###
$ echo 0 > /dev/myled0
###5秒間点灯して消灯###
$ echo 2 > /dev/myled0
```

# デモ
https://www.youtube.com/watch?v=P-YhCF_qUEo
