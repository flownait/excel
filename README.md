# excel
This is to track and record all the excel tricks


* Contain text from a list or range

If C2 to C10 is a list of text for A2 to A100 to find from, below function in B2 can be applied
```
=IF(OR(COUNTIF(A2,"*"&$C$3:$C$10&"*")), "Yes", "")
```
Or if want to list the mapped texts, then B2 can be applied with
```
=TEXTJOIN(", ", TRUE, IF(COUNTIF(A2, "*"&$C$3:$C$10&"*"), $C$2:$C$10, ""))
```


* Others...
  * Test
  * Test
