=COUNTIFS('اجتماعات'!$G:$G,">="&DATE(YEAR(MIN('اجتماعات'!$G:$G)),ROWS($AY$106:AY106),1),'اجتماعات'!$G:$G,"<"&EDATE(DATE(YEAR(MIN('اجتماعات'!$G:$G)),ROWS($AY$106:AY106),1),1))

=MIN('اجتماعات'!$G:$G)
