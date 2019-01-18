# myled2
ロボットシステム学課題1  
RaspberryPiのデバイスドライバを作りLEDを発光させる。  
Pi3 ModelBでOSはRaspbianを使用。  
LEDはGPIO25(22番ピン)に接続する。  
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

# 参考
[カーネルモジュール作成によるlinuxカーネル開発入門 - 第二回 一定時間後に処理をする(タイマー)]https://qiita.com/satoru_takeuchi/items/254dbd7bcad392263c85)
