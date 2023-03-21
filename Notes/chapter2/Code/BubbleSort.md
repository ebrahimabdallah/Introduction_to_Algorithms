
```
<?php
function bubble_sort($A)
{
    $n=sizeof($A);
    for ($i=0; $i <$n ; $i++)
     { 
        $swapped=False;
        for ($j=0; $j<$n-$i-1 ; $j++) { 
			if ($A[$j] > $A[$j+1])
            {
                $t=$A[$j];
                $A[$j]=$A[$j+1];
                $A[$j+1]=$t;
                $swapped=True;
            }
        }
        if($swapped==False)
        break;
     }
}
$A = array(64, 34, 25, 12, 22, 11, 90);
$len = sizeof($A);
bubble_sort($A);
echo "Array after sorted : \n";
for($i = 0; $i < $len; $i++)
	echo $A[$i]." ";
	
?>
```
