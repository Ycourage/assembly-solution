
六、综合类

1.根据欧几里德辗转相除法求两个正整数M、N的最大公约数R。 

2.简化的歌德巴赫猜想：任何一个大于6的偶数均可以表示为两个素数之和。现从键盘 输入一个0～65535之间的无符号整数，试验证歌德巴赫猜想。
如输入数12，输出： 12=5+7 如输入数20,输出： 20=3+17 20=7+13 如输入数7,输出： Must be even 如输入数3,输出： Must be greater than or equal to 6 

3.用减奇数次数的方法，求一个数的近似平方根，这个平方根是一个整数。如求17的平 方根，可以用17相继减去奇数1、3、5、7、…，当结果为负数时停止，即： 17-1-3-5-7-9＜0 可以看出，17 在减去 5 次奇数后结果变为负数，可以近似认为 17 的平方根在 4 与 5 之间， 计算 NUM 的平方根，如果 NUM=17，则 ANS 中保存结果 4。

4.以下面形式定义一个长整数，其所占用字节数由 N 得到，比如 128 位的数 5746352413DE89674523BC9A78563412H 定义成： NUM DB 12H,34H,56H,78H,9AH,0BCH,23H,45H DB 67H,89H,0DEH,13H,24H,35H,46H,57H N DB $-NUM 试编写一个程序，实现对 N 字节的 NUM 的值求补，并把求补后的值仍保存在 NUM 中。 

5.根据《中华人民共和国国家标准GB 11643-1999》中有关公民身份号码的规定，公民 身份号码是特征组合码，由十七位数字本体码和一位数字校验码组成。排列顺序从左至右依 次为：六位数字地址码，八位数字出生日期码，三位数字顺序码和一位数字校验码。顺序码 的奇数分给男性，偶数分给女性。校验码是根据前面十七位数字码，按照ISO 7064:1983.MOD 11-2校验码计算出来的检验码。 下面介绍计算校验码的算法: 先引入公式： (右边最低位为第 1 位，左边最高位为第 18 位)
有了 Wi 值表后，可以简化 S 的计算过程，得出 S 后计算余数 Y，Y 的计算公式为：Y = mod(S, 11)，再根据下表找出 Y 对应的校验码即为要求身份证号码的校验码 C。
编写一个程序，完成从键盘上输入一个 17 位的身份证号（身份证号的前 17 位，即上面 描述中的第 18 位至第 2 位），通过计算补充第 1 位后，将完整的身份证号显示出来。