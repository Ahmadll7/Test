Private Sub Worksheet_Change(ByVal Target As Range)

    If Intersect(Target, Me.Range("K1:K2")) Is Nothing Then Exit Sub

    UpdateMDRSColor

End Sub


Private Sub UpdateMDRSColor()

    Dim Value As Variant

    Value = Me.Range("BE41").Value

    With Me.Shapes("TextBox 47").TextFrame2.TextRange.Font.Fill.ForeColor

        If IsNumeric(Value) Then

            If Value > 0 Then
                .RGB = RGB(0, 176, 80)

            ElseIf Value < 0 Then
                .RGB = RGB(192, 0, 0)

            Else
                .RGB = RGB(0, 0, 0)

            End If

        Else
            .RGB = RGB(0, 0, 0)

        End If

    End With

End Sub
