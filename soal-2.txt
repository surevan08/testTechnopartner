<?php

$huruf = array("A", "B", "C", "D", "E", "C", "F", "Z");
$nilai = null;
for ($i = 0; $i < 1000; $i++) {
    for ($x = $i + 1; $x < count($huruf); $x++) {
        if ($nilai) {
            break;
        } elseif ($huruf[$i] == $huruf[$x]) {
            $nilai = $huruf[$i];
        }
    }
}

if ($nilai != null) {
    echo "Output : " . $nilai;
} else {
    echo "Output : false";
}
