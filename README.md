### RoboSys_kadai1

2020ロボットシステム学_課題１

### 概要
Raspberry piとLEDランプを用いてLEDを点灯・点滅させる.

echo 1でLED点灯,
echo 0でLED消灯,
echo 2でLEDが1秒間隔で点滅,
echo 3でLEDが2秒間隔で点滅.


### 動作環境
|||
|:--:|:--:|
| Raspberry Pi | Raspberry Pi Model 3B+ |
| OS | Ubuntu16.04 |
| GPIO25 | 22番ピン |
| GND | 39番ピン |

### インストール方法
```
$ git clone 
$ cd myled
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
```
### 実行方法
```
$ echo 1 > /dev/myled0
$ echo 0 > /dev/myled0
$ echo 2 > /dev/myled0
$ echo 3 > /dev/myled0
```
### デバイスドライバのアンインストール
```
$ sudo rmmod myled0

```
### 動画のリンク
https://youtu.be/zS5DF9D2wYA
