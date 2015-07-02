# 0702
js作用域
<!DOCYYPE html>
<html>
 <head>
  <title>Test</title>
    <meta http-equiv="Content-Type" content="text/html;charset=utf-8" >
   </head>
   <script type="javascript/text">
     var scope="global scope";
     function f1()
     {
       var scope="local scope";
       function f2()
       {
         var scope="nested scope";
         return scope;
       }
       return f2();
     }
     f1();//nested scope
    </script>
    <body>
    </body>
    </html>
