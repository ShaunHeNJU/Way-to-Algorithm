<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>

# Decimal Conversion - 进制转换

--------

#### 问题

将整数$$ x $$从$$ a $$进制转化为$$ b $$进制（其中$$ 2 \le a, b \le 32 $$）。

#### 解法

$$ (1) $$模拟加法运算的过程将数字$$ x_a = [ 8, 3, 7, 1 ]\_a $$转换为$$ y_{b} = [ 8, 3, 7, 1 ]_{b} $$，有$$ y[i]_{b} = x[i]_{a} \cdot a^i % b^i $$，$$ y[i+1]_{b} = y[i+1]_{b} + ( x[i]_{a} \times a^i \div b^i ) $$。

$$ (1) $$模拟减法运算的过程将数字$$ x_a = [ 8, 3, 7, 1 ]\_a $$转换为$$ y_{b} = [ 8, 3, 7, 1 ]_{b} $$，有$$ y[i]_{b} = x[i]_{a} \cdot a^i % b^i $$，$$ y[i+1]_{b} = y[i+1]_{b} + ( x[i]_{a} \times a^i \div b^i ) $$。

--------

#### 源码

[DecimalConversion.h](https://github.com/linrongbin16/Way-to-Algorithm/blob/master/src/Calculation/DecimalConversion.h)

[DecimalConversion.h](https://github.com/linrongbin16/Way-to-Algorithm/blob/master/src/Calculation/DecimalConversion.cpp)

#### 测试

[DecimalConversionTest.h](https://github.com/linrongbin16/Way-to-Algorithm/blob/master/src/Calculation/DecimalConversionTest.cpp)
