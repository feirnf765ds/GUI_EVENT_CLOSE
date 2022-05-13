# GUI_EVENT_CLOSE
Exit Case $hPause ; Pause button ConsoleWrite("!Pause" &amp; @LF) _Pause() EndSwitch WEnd Func _Pause() GUICtrlSetData($hPause, "Resume") While 3 Switch GUIGetMsg() Case -3 ; $GUI_EVENT_CLOSE need to be able to exit while paused. Exit Case $hPause ; Pause button ExitLoop EndSwitch WEnd
