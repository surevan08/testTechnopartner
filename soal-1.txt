<?php

$angka = array(-0.5, -0.76, 0.45, -0.2, 4.5, 3.5);
$nilai = null;

for ($i = 0; $i < 1000; $i++) {
    for ($x = $i + 1; $x < count($angka); $x++) {
        if ($angka[$i] > $angka[$x]) {
            $nilai = $angka[$i];
            $nilais = $angka[$x];
        }
    }
}

echo 'Output : ' . $nilais;
