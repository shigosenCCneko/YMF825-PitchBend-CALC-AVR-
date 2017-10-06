# YMF825_MIDI_HID
YMF825 MIDI　Player　USB　MIDI-HID複合デバイス
    
    Atmega32U4

		calc_exp ピッチベンド値の計算
		
    uint16_t calc_exp( uint16_t num, uint8_t range)
		num:	pitchbend 14bitを(計算は上位10bit )
		range:  0-24 (0:無し 24±２オクターブ)
    
    戻り値 (2.14)形式の固定小数点,bit15-11を#18,bit10-5を#19へ分ける

