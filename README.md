=IF($K$1="الكل",IF($K$3="الكل",INDEX(استفسارات!$Q$4:$AB$4,1,ROWS($BA$21:BA21)),IF(OR(INDEX($AV$21:$AV$32,ROWS($BA$21:BA21))=$K$3,INDEX($AW$21:$AW$32,ROWS($BA$21:BA21))=$K$3),INDEX(استفسارات!$Q$4:$AB$4,1,ROWS($BA$21:BA21)),"")),IF(ROWS($BA$21:BA21)=1,IF(OR($K$3="الكل",INDEX($AV$21:$AV$32,MATCH($K$1,$AX$21:$AX$32,0))=$K$3,INDEX($AW$21:$AW$32,MATCH($K$1,$AX$21:$AX$32,0))=$K$3),$K$1,""),""))




=IF(BA21="","",IF($K$1="الكل",IF($K$3="الكل",INDEX(استفسارات!$Q$11:$AB$11,1,ROWS($BB$21:BB21)),INDEX(استفسارات!$Q$11:$AB$11,1,ROWS($BB$21:BB21))*--((INDEX($AV$21:$AV$32,ROWS($BB$21:BB21))=$K$3)+(INDEX($AW$21:$AW$32,ROWS($BB$21:BB21))=$K$3)>0)),INDEX(استفسارات!$Q$11:$AB$11,1,MATCH($K$1,استفسارات!$Q$4:$AB$4,0))))
