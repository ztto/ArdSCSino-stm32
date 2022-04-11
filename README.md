# ArdSCSino-stm32

ArdSCSino-stm32 とは たんぼ（TNB製作所）(https://twitter.com/h_koma2) さんが作成した ArdSCSino のSTM32版です<br>
ArdSxSino とは SCSI(SASI)デバイス（ハードディスク）を arduino で再現するハードウエアです。<br>
許可を頂いて公開することになりました。<br>

X68000 のSASI対応<br>
注意１．ACE、EXPERTでは動作していますがPROではDSKBENCHが終了しない等問題があります<br>
注意２．SHARP X1turbo、NEC PC98、での動作確認が出来ていません<br>

「scsi-config.txt」ファイルに各種パラメータを記述できるようになりました<br>
　※サンプルを置いています<br>
記述方法<br>
・１列目：ベンダ名　　　半角8文字<br>
・２列目：プロダクト名　半角16文字<br>
・３列目：バージョン　　半角4文字<br>
・４列目：タイプ　　　　半角1文字  <0 for STANDARD, 1 for SHARP X1turbo, 2 for NEC PC98><br>
・５列目：WAIT時間　　　半角3文字  <SASIは、80 程度の値を入れて異常終了しない値を設定する><br>

例）･は半角空白と思ってください<br>
--------------<br>
NECGATE･<br>
ST410800N･･･････<br>
1.0･<br>
0<br>
000<br>
--------------<br>

# Setup<br>
* platformio を使用しています。<br>

 マイクロSDCARDアダプタとして以下を使用しています。<br>

 Hirose DM3AT-SF-PEJM5<br>

