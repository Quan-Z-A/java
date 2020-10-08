# java
java lab
## 实验内容
基本要求：完成教材p110 第四题关于PC、内存等模拟的程序。
附加要求：
类中定义不少于两个构造方法；
每个类定义不少于2个属性，且属性的类型应该多样化；
根据课堂中关于访问权限的内容，尝试定义属性的修饰符多样化，类中定义方法操作属性，避免直接通过“类对象.属性”的形式访问属性值；且定义的方法内应该有符合常理的逻辑判断；
尝试把本次实验的多个类放置在不同的包中，体会修饰符private的用法。

## 实验过程
创建test主类 cpu harddisk pc类并赋值
## 实验方法
在test创建cpu disk pc对象并设置数值 cpu类返回speed值，setspeed(int m)将m赋值给speed；harddisk类返回amount值；pc类setcpu（cpu c）赋值给cpu，setharddisk（harddisk h）赋值给hd。
show（）显示cpu和硬盘性能

## 核心代码
```
package pack1;

public class Text {
 public static void main(String args[]) {
   //创建一个CPU对象
  CPU cpu =new CPU();
   //将cpu的speed设置为2200
     cpu.setSpeed(2200);
   //cpu型号  
     cpu.settype("i7-9750H");
   //创建一个HardDisk对象
     HardDisk disk=new HardDisk();
   //将disk的amount设置为200
     disk.setAmount(200);
   //硬盘读写速度  
     disk.setspeed2(500);
   //创建一个PC对象
     PC pc=new PC();
     pc.setCPU(cpu);
     pc.setHardDisk(disk);
     pc.show();
  }
   
  
}
```
## 实验结果
![](java实验结果.png)
## 实验感想
熟悉了类的创建及基本数据类型使用，学会了类的组合与复用
