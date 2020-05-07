# B10856031.github.io

<html>

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>科科快餐點餐價格表</title>

    <style>
        h1 {
            font-size: 36px;
            font-weight: bolder;
            color: blue;
            text-align: center;
        }
        
        table {
            margin: auto;
            border: 1px;
            border-style: dashed;
        }
        
        td {
            border-style: dotted;
            border-width: 1px;
            padding: 10px;
            color: green;
        }
        
        .td_noBorder {
            border-width: 0px;
        }
        
        .content {
            color: green;
            font-family: Arial;
            font-size: 18px;
        }
        
        #tableTitle {
            font-weight: bolder;
            font-size: 18px;
            color: purple;
            text-align: center
        }
    </style>
    <script>
        var x, y, a;
        document.write("<center>");
        document.write("<h1>MIS快餐點餐價格表</h1>");
        document.write("<table>");
        for (y = 2; y <= 7; y++) {
            document.write("<tr>");
            for (x = 5, a = 6; x <= 20; x += 3, a--) {
                if (y == 2 && x == 5) { //最左上那格
                    document.write("<td class='td_noBorder'>");
                    document.write("</td>");
                } else if (y == 2 && x != 5) { //第一排2~6格
                    document.write("<td id='tableTitle'>");
                    document.write(a + '號餐<br>' + x + '元');
                    document.write("</td>");
                } else { //第2~6排第一格
                    if (x == 5) {
                        document.write("<td id='tableTitle'>");
                        document.write(y);
                        document.write("</td>");
                    } else { //中間綠字的部分
                        document.write("<td class='content'>");
                        document.write(y + '*' + x + '=' + x * y);
                        document.write("</td>");
                    }
                }
            }
            document.write("</tr>");
        }
        document.write("</table>");
        document.write("</center>");
    </script>
</head>

<body>
</body>

</html>
