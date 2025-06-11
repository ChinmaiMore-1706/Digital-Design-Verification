## implementation of dynamic array

>```
>module tb;
>  int dyn1[];
>  int dyn2[4][];
>  initial begin
>    dyn1=new[10];
>    foreach (dyn1[i])
>      dyn1[i]=$random;
>    dyn1=new[20](dyn1);
>    dyn1=new[50];
>  $display("dyn1=%p,dyn2=%p",dyn1,dyn2);
>  end
>endmodule
>```
>
>```
>•	OUTPUT : dyn1='{0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0} ,
>•	dyn2='{'{}, '{}, '{}, '{}}
>```

## implementation of associative array
>```
> •	CODE:
> module test;
 > int a[int];
 > initial begin
 > a[500]=100;
  > $display("size=%d",a.size());
  > end
> endmodule
>
>•	OUTPUT :     size=          1
>```


