<?php

$huruf = array(1, 2, 4, 4, 5, 6, 7, 7, 8, 8);
$nilai = 12;
$nilai1 = null;
$nilai2 = null;
for ($i = 0; $i < 1000; $i++) {
    if ($nilai1 == true && $nilai2 == true) {
        break;
    } else {
        for ($x = $i + 1; $x < count($huruf); $x++) {
            if ($nilai1 == true && $nilai2 == true) {
                break;
            } elseif (($huruf[$i] + $huruf[$x]) == $nilai) {
                $nilai1 = $huruf[$i];
                $nilai2 = $huruf[$x];
            }
        }
    }
}

if ($nilai1 != null && $nilai2 != null) {
    echo "True ( Karena " . $nilai1 . " + " . $nilai2 . " = " . $nilai . " )";
} else {
    echo "False ( Tidak ada pasangan yang dijumlah = " . $nilai . "  )";
}
