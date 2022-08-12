Public Class Form1

    Dim p1 As Integer
    Dim p2 As Integer
    Dim p3 As Integer
    Dim p4 As Integer
    Dim p5 As Integer
    Dim P6 As String
    Dim P7 As String
    Dim p8 As Integer
    Dim p9 As Integer
    Dim p10 As Integer
    Dim p11 As Integer
    Dim p12 As Integer
    Dim P13 As String
    Dim P14 As String

    Dim data1 As String
    Dim data2 As String
    Dim data3 As String
    Dim data4 As String
    Dim data5 As String
    Dim data6 As String
    Dim data7 As String
    Dim data8 As String
    Dim data9 As String
    Dim data10 As String
    Dim data11 As String
    Dim data12 As String
    Dim data13 As String
    Dim data14 As String
    Dim data15 As String


    Dim M1_1_COUNT As Integer = 0
    Dim M1_2_COUNT As Integer = 0
    Dim M1_3_COUNT As Integer = 0
    Dim M1_4_COUNT As Integer = 0
    Dim M1_5_COUNT As Integer = 0
    Dim M1_Totol As Integer



    Dim Data_Count_print_lable As String


    Dim x As Integer
    Dim Serial_lock As Integer = 0



    Private Sub Form1_Load(sender As Object, e As EventArgs) Handles MyBase.Load


        SerialPort1.Open()
        SerialPort1.DtrEnable = True
        Timer1.Start()


    End Sub

    Private Sub Timer1_Tick(sender As Object, e As EventArgs) Handles Timer1.Tick





        '  TextBox1.Text = SerialPort1.ReadExisting

        If TextBox1.Text <> "" And Len(TextBox1.Text) > 1 Then TextBox2.Text = TextBox1.Text


        p1 = InStr(TextBox2.Text, TextBox14.Text) ''''A / AKURA
        TextBox3.Text = p1
        data1 = Mid(TextBox2.Text, p1 + 1)
        TextBox5.Text = Val(data1)
        ' If (TextBox4.Text >= "") Then TextBox5.Text = TextBox4.Text
        ' If (p1 = 1) Then TextBox5.Text = TextBox4.Text


        rack_1_1.Text = M1_1_COUNT
        rack_1_2.Text = M1_2_COUNT
        rack_1_3.Text = M1_3_COUNT
        rack_1_4.Text = M1_4_COUNT
        rack_1_5.Text = M1_5_COUNT
        M1_Totol = M1_1_COUNT + M1_2_COUNT + M1_3_COUNT + M1_4_COUNT + M1_5_COUNT
        M1_TOTAL_lable.Text = M1_Totol
       


        If Data_Count_Lable.Text = "1" Then M1_1_COUNT = Val(data1)
        If Data_Count_Lable.Text = "2" Then M1_2_COUNT = Val(data1)
        If Data_Count_Lable.Text = "3" Then M1_3_COUNT = Val(data1)
        If Data_Count_Lable.Text = "4" Then M1_4_COUNT = Val(data1)
        If Data_Count_Lable.Text = "5" Then M1_5_COUNT = Val(data1)


        '////////////////////////////////////


        Timer3.Start()
        Timer1.Stop()


        '  Data_Count.PerformClick()


        ' rack_1_1.Text = TextBox5.Text


        '  p2 = InStr(TextBox2.Text, TextBox15.Text) ''''B / AKURA
        '  TextBox19.Text = p2
        '  data2 = Mid(TextBox2.Text, p2 + 1)
        ' TextBox6.Text = Val(data2)
        ' If (TextBox6.Text >= "") Then TextBox7.Text = TextBox6.Text
        ' If (p2 = 1) Then TextBox7.Text = TextBox6.Text



        '  p3 = InStr(TextBox2.Text, TextBox16.Text) ''''C / AKURA
        '  TextBox20.Text = p3
        '  data3 = Mid(TextBox2.Text, p3 + 1)
        ' TextBox8.Text = Val(data3)
        ' If (TextBox8.Text >= "") Then TextBox9.Text = TextBox8.Text
        '  If (p3 = 1) Then TextBox9.Text = TextBox8.Text


        '  p4 = InStr(TextBox2.Text, TextBox17.Text) ''''D / AKURA
        '  TextBox21.Text = p4
        '  data4 = Mid(TextBox2.Text, p4 + 1)
        '  TextBox10.Text = Val(data4)
        '  If (TextBox10.Text >= "") Then TextBox11.Text = TextBox10.Text
        '  If (p4 = 1) Then TextBox11.Text = TextBox10.Text


        ' p5 = InStr(TextBox2.Text, TextBox18.Text) ''''E / AKURA
        '  TextBox22.Text = p5
        '  data5 = Mid(TextBox2.Text, p5 + 1)
        '  TextBox12.Text = Val(data5)
        '  If (TextBox12.Text >= "") Then TextBox13.Text = TextBox12.Text
        '  If (p5 = 1) Then TextBox13.Text = TextBox12.Text




        '  P6 = InStr(TextBox2.Text, T1.Text) ''''F / AKURA
        '  T2.Text = P6
        '  data6 = Mid(TextBox2.Text, P6 + 1)
        '  T3.Text = Val(data6)
        '  If (T3.Text >= "") Then T4.Text = T3.Text
        '  If (P6 = 1) Then T4.Text = T3.Text


        '  P7 = InStr(TextBox2.Text, T5.Text) ''''G / AKURA
        '  T6.Text = P7
        '  data7 = Mid(TextBox2.Text, P7 + 1)
        '  T7.Text = Val(data7)
        ' If (T7.Text >= "") Then T8.Text = T7.Text
        ' If (P7 = 1) Then T8.Text = T7.Text




        '  p8 = InStr(TextBox2.Text, T9.Text) ''''H / AKURA
        ' T10.Text = p8
        ' data8 = Mid(TextBox2.Text, p8 + 1)
        ' T11.Text = Val(data8)
        ' If (T11.Text >= "") Then T12.Text = T11.Text
        '  If (p8 = 1) Then T12.Text = T11.Text



        'Button1.Location = New Point(125, TextBox5.Text)




    End Sub

    Private Sub Button1_Click(sender As Object, e As EventArgs)




    End Sub

    Private Sub Button1_Click_1(sender As Object, e As EventArgs)

        '  Serial_lock = "1"
        '  SerialPort1.Close()

    End Sub

    Private Sub Button1_Click_2(sender As Object, e As EventArgs)

    End Sub

    Private Sub bt2_Click(sender As Object, e As EventArgs)





    End Sub

    Private Sub Button2_Click(sender As Object, e As EventArgs)



    End Sub

    Private Sub Button8_Click(sender As Object, e As EventArgs)


        ' SerialPort1.Write("A")


    End Sub

    Private Sub Label5_Click(sender As Object, e As EventArgs) Handles Label5.Click

        ' Button10.Visible = True
        Form2.Show()
        ' Button10.Location = New Point(1327, 1)


    End Sub

    Private Sub Button3_Click(sender As Object, e As EventArgs) Handles Button3.Click

    End Sub

    Private Sub Timer2_Tick(sender As Object, e As EventArgs) Handles Timer2.Tick

    End Sub

    Private Sub TextBox7_TextChanged(sender As Object, e As EventArgs)

    End Sub

    Private Sub TextBox4_TextChanged(sender As Object, e As EventArgs)

    End Sub

    Private Sub TextBox15_TextChanged(sender As Object, e As EventArgs)

    End Sub

    Private Sub TextBox3_TextChanged(sender As Object, e As EventArgs) Handles TextBox3.TextChanged

    End Sub

    Private Sub TextBox2_TextChanged(sender As Object, e As EventArgs) Handles TextBox2.TextChanged

    End Sub

    Private Sub TextBox1_TextChanged(sender As Object, e As EventArgs) Handles TextBox1.TextChanged

    End Sub

    Private Sub TextBox14_TextChanged(sender As Object, e As EventArgs) Handles TextBox14.TextChanged

    End Sub



    Private Sub Data_Count_Click(sender As Object, e As EventArgs) Handles Data_Count.Click


       


        Data_Count_print_lable = Data_Count_print_lable + 1
        Data_Count_Lable.Text = Data_Count_print_lable


        If Data_Count_print_lable = 1 Then SerialPort1.Write("A")
        If Data_Count_print_lable = 2 Then SerialPort1.Write("B")
        If Data_Count_print_lable = 3 Then SerialPort1.Write("C")
        If Data_Count_print_lable = 4 Then SerialPort1.Write("D")
        If Data_Count_print_lable = 5 Then SerialPort1.Write("E")


        If Data_Count_print_lable >= 5 Then Data_Count_print_lable = 0







    End Sub



    Private Sub Timer3_Tick(sender As Object, e As EventArgs) Handles Timer3.Tick


        Data_Count_print_lable = Data_Count_print_lable + 1
        Data_Count_Lable.Text = Data_Count_print_lable




        If Data_Count_print_lable = 1 Then SerialPort1.Write("A")
        If Data_Count_print_lable = 2 Then SerialPort1.Write("B")
        If Data_Count_print_lable = 3 Then SerialPort1.Write("C")
        If Data_Count_print_lable = 4 Then SerialPort1.Write("D")
        If Data_Count_print_lable = 5 Then SerialPort1.Write("E")


        If Data_Count_print_lable >= 5 Then Data_Count_print_lable = 0


        TextBox1.Text = SerialPort1.ReadExisting

        Timer3.Stop()
        Timer1.Start()


    End Sub

    Private Sub T9_TextChanged(sender As Object, e As EventArgs)

    End Sub

    Private Sub bt1_TextChanged(sender As Object, e As EventArgs)
    End Sub

    Private Sub Button11_Click(sender As Object, e As EventArgs)
    End Sub

    Private Sub rack_1_5_Click(sender As Object, e As EventArgs) Handles rack_1_5.Click

    End Sub

    Private Sub rack_1_4_Click(sender As Object, e As EventArgs) Handles rack_1_4.Click

    End Sub

    Private Sub rack_1_3_Click(sender As Object, e As EventArgs) Handles rack_1_3.Click

    End Sub

    Private Sub rack_1_2_Click(sender As Object, e As EventArgs) Handles rack_1_2.Click

    End Sub

    Private Sub rack_1_1_Click(sender As Object, e As EventArgs) Handles rack_1_1.Click

    End Sub

    Private Sub M1_TOTAL_lable_Click(sender As Object, e As EventArgs) Handles M1_TOTAL_lable.Click

    End Sub
End Class


<!---
Uditha1123/Uditha1123 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
