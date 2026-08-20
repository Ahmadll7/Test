Private Sub Worksheet_Change(ByVal Target As Range)

    If Intersect(Target, Me.Range("K1:K2")) Is Nothing Then Exit Sub

    On Error GoTo ExitHandler
    Application.EnableEvents = False

    UpdateMDRSColor

ExitHandler:
    Application.EnableEvents = True

End Sub


Private Sub UpdateMDRSColor()

    Dim txt As String

    txt = Me.Range("BE41").Value

    With Me.Shapes("TextBox 14").TextFrame.Characters.Font

        If Left(txt, 1) = "▲" Then
            .Color = RGB(0, 176, 80)

        ElseIf Left(txt, 1) = "▼" Then
            .Color = RGB(192, 0, 0)

        Else
            .Color = RGB(0, 0, 0)

        End If

    End With

End Sub
