# 設定値

## Address

0〜0xFFFFの範囲。10進数で、0〜65535の範囲。

## Channel

Bandwidthによって、設定できるチャンネル値が変わります。

| Channel | Bandwidth(kHz) |
|:--|:--|
| 0-37  | 125kHz |
| 0-36  | 250kHz |
| 0-30  | 500kHz |

## LR(LoRa Rate)

転送レートやSF値、バンド幅は下記値で設定できます。

| Value | 伝送レート(bps) | SF | Bandwidth(kHz) |
|:--|:--|:--|:--|
| 0 | 15625 bps | SF5 | 125kHz |
| 4 | 9375 bps | SF6 | 125kHz |
| 6 | 5469 bps | SF7 | 125kHz |
| 12 | 3125 bps | SF8 | 125kHz |
| 16 | 1758 bps | SF9 | 125kHz |
| 1 | 31250 bps | SF5 | 250kHz |
| 5 | 18750 bps | SF6 | 250kHz |
| 9 | 10938 bps | SF7 | 250kHz |
| 13 | 6520 bps | SF7 | 250kHz |
| 17 | 3516 bps | SF8 | 250kHz |
| 21 | 1953 bps | SF9 | 250kHz |
| 2 | 62500 bps | SF5 | 500kHz |
| 6 | 37500 bps | SF6 | 500kHz |
| 10 | 21875 bps | SF7 | 500kHz |
| 14 | 12500 bps | SF8 | 500kHz |
| 18 | 7031 bps | SF9 | 500kHz |
| 22 | 3906 bps | SF9 | 500kHz |
| 26 | 2148 bps | SF9 | 500kHz |


## Send Mode

Send Modeでは、トランスペアレント送信モードと固定送信モードが選択できます。トランスペアレント送信モードでは、同じアドレス, 同じチャンネルを設定した端末に一斉に送信されます。固定送信モードでは、指定したアドレス、指定したチャンネルの端末にデータ送信できます。

| Value | モード |
|:--|:--|
| 0 | トランスペアレント送信モード |
| 1 | 固定送信モード |

## RSSI

RSSIバイトの有効化をおこなうと、RSSI強度も出力されます。

RSSIからdBmへの変換は

	dBm = - (256 - RSSI)

## Power

Powerでは送信出力電力を設定できます。

| Value | 電力 |
|:--|:--|
| 0 | 13dBm |
| 1 | 12dBm |
| 2 | 7dBm |
| 3 | 0dBm |

