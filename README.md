Sub UpdateMDRSColor()

    Dim txt As String

    txt = Worksheets("dashboard").Range("BE41").Value

    With Worksheets("dashboard").Shapes("TextBox 14").TextFrame2.TextRange.Font.Fill.ForeColor

        If Left(txt, 1) = "▲" Then
            .RGB = RGB(0, 176, 80)

        ElseIf Left(txt, 1) = "▼" Then
            .RGB = RGB(192, 0, 0)

        Else
            .RGB = RGB(0, 0, 0)

        End If

    End With

End Sub
