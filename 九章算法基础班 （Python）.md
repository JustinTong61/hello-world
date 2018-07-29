# 九章算法基础班 （Python）
37. Reverse 3-digit Integer
![](%E4%B9%9D%E7%AB%A0%E7%AE%97%E6%B3%95%E5%9F%BA%E7%A1%80%E7%8F%AD%20%EF%BC%88Python%EF%BC%89/37.%20%E5%8F%8D%E8%BD%AC%E4%B8%80%E4%B8%AA3%E4%BD%8D%E6%95%B4%E6%95%B0%20-%20LintCode%20Google%20Chrome,%20Today%20at%201.03.47%20PM.png)

``` py.   
class Solution:
    """
    @param number: A 3-digit number.
    @return: Reversed number.
    """
    def reverseInteger(self, number):
        # write your code here
        digit1=number%10
        digit2=number//10%10
        digit3=number//100
        return digit1*100+digit2*10+digit3
```

* 从reverseInteger （）即为自己的code
* 要注意的是number为已经define好的变量
* digit1的%为求余数 比如123%10 余数为3                                                                                                                                                                                                                                                                                                                                                                                                                  
* digit2的为取下整数 123/_10的下整数为12 对于负数取下证小心 比如-7_/4=-2
* 最后要输出number 既return 可以先先number=blabla 再return number

766. Leap Year
![](%E4%B9%9D%E7%AB%A0%E7%AE%97%E6%B3%95%E5%9F%BA%E7%A1%80%E7%8F%AD%20%EF%BC%88Python%EF%BC%89/766.%20%E9%97%B0%E5%B9%B4%20-%20LintCode%20Google%20Chrome,%20Today%20at%201.02.20%20PM.png)

``` py.   
class Solution:
    """
    @param n: a number represent year
    @return: whether year n is a leap year.
    """
    def isLeapYear(self, n):
        # write your code here
        if n%4==0 and n%100!=0 or n%400==0:
            return True
        else:
            return False
        
```

* 此题首先明白输出的是什么类型 是否为闰年 那么输出为boolean
* 此次要做判断，所以要用if statement
* 细节要注意的即Python和其他语法的不同

