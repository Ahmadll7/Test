=IF($K$1="الكل",INDEX('استفسارات'!$C$34:$N$34,1,ROWS($BI$21:BI21)),IF(ROWS($BI$21:BI21)=1,$K$1,""))



=IF(BI21="","",IF($K$2="الكل",INDEX('استفسارات'!$C$40:$N$40,1,MATCH(BI21,'استفسارات'!$C$34:$N$34,0)),INDEX('استفسارات'!$C$35:$N$39,MATCH($K$2,'استفسارات'!$B$35:$B$39,0),MATCH(BI21,'استفسارات'!$C$34:$N$34,0))))



ClassificationMonths
=dashboard!$BI$21:INDEX(dashboard!$BI$21:$BI$32,IF(dashboard!$K$1="الكل",12,1))


ClassificationValues
=dashboard!$BJ$21:INDEX(dashboard!$BJ$21:$BJ$32,IF(dashboard!$K$1="الكل",12,1))


='Dashboard'!ClassificationValues
='Dashboard'!ClassificationMonths
