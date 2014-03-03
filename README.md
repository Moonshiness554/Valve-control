Valve-control
-=============-

' {$STAMP BS2}
' {$PBASIC 2.5}

ValvePin CON 14
counter VAR Word

counter = 0

DEBUG "Program Running", CR

DO
LOOP UNTIL IN0 = 1

DO
LOOP UNTIL IN0 = 0

DEBUG "asyuh", CR

HIGH ValvePin

DO
counter = counter + 1
LOOP UNTIL IN0 = 1

DEBUG "asdyuaosi", CR

LOW ValvePin

DEBUG DEC counter

END
