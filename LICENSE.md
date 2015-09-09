 //应用FileInputStream类，编写应用程序，从磁盘上读取一个Java程序，并将源程序代码显示在屏幕上。
 （被读取的文件路径为：E:/myjava/Hello.java）

// Programme Name FISDemo.java
import java.io.*;
  public class FISDemo {
  public static void main(String args[]) {
    byte[] buf=new byte[2056];
    try{
     FileInputStream fileIn=new FileInputStream("e:/myjava/Hello.java");
     int bytes=fileIn.read(buf,0,2056);
     String str=new String(buf,0,bytes);
     System.out.println(str);
}catch(Exception e){
 e.printStackTrace( );
}
}
