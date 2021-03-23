# excel
This is to track and record all the excel tricks


* Contain text from a list or range [Reference](https://www.get-digital-help.com/if-cell-contains-text-from-list/)

If C2 to C10 is a list of text for A2 to A100 to find from, below function in B2 can be applied
```
=IF(OR(COUNTIF(A2,"*"&$C$3:$C$10&"*")), "Yes", "")
```
Or if want to list the mapped texts, then B2 can be applied with
```
=TEXTJOIN(", ", TRUE, IF(COUNTIF(A2, "*"&$C$3:$C$10&"*"), $C$2:$C$10, ""))
```

* Sum specific columns or rows or both [Reference!](https://www.get-digital-help.com/if-cell-contains-text-from-list/)

If RawData is a defined range (e.g. A2:AA1000),  is a list of text for A2 to A100 to find from, below function in B2 can be applied
```
=SUMPRODUCT(INDEX(RawData,,MATCH($F2,'Sheet 1'!$K$1:$BK$1,0)),--(P1='Sheet 2'!$D271),--(P2='Sheet 2'!$H271),--(P3='Sheet 2'!I$5))
```




* Others...
  * Test
  * Test
