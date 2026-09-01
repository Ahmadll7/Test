=IF($K$1="الكل",IF($K$3="الكل",INDEX(استفسارات!$C$34:$N$34,1,ROWS($BI$21:BI21)),IF(OR(INDEX($AV$21:$AV$32,ROWS($BI$21:BI21))=$K$3,INDEX($AW$21:$AW$32,ROWS($BI$21:BI21))=$K$3),INDEX(استفسارات!$C$34:$N$34,1,ROWS($BI$21:BI21)),"")),IF(ROWS($BI$21:BI21)=1,$K$1,""))


=IF(BI21="","",IF($K$1="الكل",IF($K$3="الكل",INDEX(استفسارات!$C$40:$N$40,1,ROWS($BJ$21:BJ21)),INDEX(استفسارات!$C$40:$N$40,1,ROWS($BJ$21:BJ21))*--((INDEX($AV$21:$AV$32,ROWS($BJ$21:BJ21))=$K$3)+(INDEX($AW$21:$AW$32,ROWS($BJ$21:BJ21))=$K$3)>0)),INDEX(استفسارات!$C$40:$N$40,1,MATCH($K$1,استفسارات!$C$34:$N$34,0))))
