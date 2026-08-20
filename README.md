Sub TestMDRSColor()

    With Worksheets("dashboard").Shapes("TextBox 14").TextFrame2.TextRange.Font.Fill.ForeColor

        .RGB = RGB(192, 0, 0)

    End With

End Sub
