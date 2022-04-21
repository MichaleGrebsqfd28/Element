# Element
Func _ArrayTranspose(ByRef $aArr)     If UBound($aArr, 0) &lt;> 2 Then         SetError(-1)         Return     EndIf     Local $element, $x = UBound($aArr, 1), $y = UBound($aArr, 2), $z = $y     If $x > $y Then $z = $x     ReDim $aArr[$z][$z]     For $i = 0 To $z - 2         For $j = $i + 1 To $z - 1             $element = $aArr[$i][$j]             $aArr[$i][$j] = $aArr[$j
