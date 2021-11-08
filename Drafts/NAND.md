# Universality
 Can simulate NOT, AND, XOR
 ## NOT
 $f(x)=NAND(x,1)\equiv NOT(x)$

## AND
$f(x,y)=NAND(NAND(x,y),1)=NOT(NAND(x,y))\equiv AND(x,y)$

## XOR
we can use NOT and AND here because we defined them as NANDs before.
$f(x,y)=AND(NAND(x,y),NAND(NOT(x),NOT(y)))$
 