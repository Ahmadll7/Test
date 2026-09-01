=IF($K$1="الكل",IF($K$3="الكل",INDEX(استفسارات!$C$26:$N$26,1,ROWS($BE$21:BE21)),IF(OR(INDEX($AV$21:$AV$32,ROWS($BE$21:BE21))=$K$3,INDEX($AW$21:$AW$32,ROWS($BE$21:BE21))=$K$3),INDEX(استفسارات!$C$26:$N$26,1,ROWS($BE$21:BE21)),"")),IF(ROWS($BE$21:BE21)=1,$K$1,""))


=IF(BE21="","",IF($K$1="الكل",IF($K$3="الكل",INDEX(استفسارات!$C$32:$N$32,1,ROWS($BF$21:BF21)),INDEX(استفسارات!$C$32:$N$32,1,ROWS($BF$21:BF21))*--((INDEX($AV$21:$AV$32,ROWS($BF$21:BF21))=$K$3)+(INDEX($AW$21:$AW$32,ROWS($BF$21:BF21))=$K$3)>0)),INDEX(استفسارات!$C$32:$N$32,1,MATCH($K$1,استفسارات!$C$26:$N$26,0))))

