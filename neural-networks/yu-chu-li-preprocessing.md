# 【预处理】Pre-Processing

## 语音信号去噪（平滑化）

### 傅里叶变换（FFT）

{% embed url="https://www.zhihu.com/question/19714540/answer/1119070975" %}

### 短时傅里叶变换（STFT）

{% embed url="https://blog.csdn.net/weixin_45317919/article/details/110910320" %}

{% embed url="https://zhuanlan.zhihu.com/p/351634228" %}

### 维纳滤波（Wiener Filter）

{% embed url="https://blog.csdn.net/Frankgoogle/article/details/105571407" %}

### Python库推荐

最后介绍一些好用的Python库，其中包括许多上述方法的快速实现

```python
import scipy.signal as signal
import numpy.fft as fft
```

