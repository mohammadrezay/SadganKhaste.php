# SadganKhaste.php
https://quera.org/problemset/3406?tab=description
<?php
$a = (int)readline("Enter a three-digit number: ");
$b = (int)readline("Enter a three-digit number: ");
$aa = (preg_split('//u', $a, null, PREG_SPLIT_NO_EMPTY));
$bb = (preg_split('//u', $b, null, PREG_SPLIT_NO_EMPTY));
$aaa = array_reverse($aa);
$bbb = array_reverse($bb);
if($aaa > $bbb){
	echo "$b < $a";
}elseif($bbb > $aaa){
	echo "$a < $b";
}else{
	echo "$a = $b";
}
