```python
import numpy as np
import matplotlib.pyplot as plt

# Define x[n] and h[n]
n_x = np.arange(3, 8+1)  # x[n] is 1 for 3 ≤ n ≤ 8
x_n = np.ones(len(n_x))

n_h = np.arange(4, 15+1)  # h[n] is 1 for 4 ≤ n ≤ 15
h_n = np.ones(len(n_h))

# Compute convolution y[n] = x[n] * h[n]
y_n = np.convolve(x_n, h_n)

# Compute the range for n (convolution range)
n_y = np.arange(n_x[0] + n_h[0], n_x[-1] + n_h[-1] + 1)

# Plot the result
plt.stem(n_y, y_n, basefmt=" ")
plt.xlabel('n')
plt.ylabel('y[n]')
plt.title('Convolution y[n] = x[n] * h[n]')
plt.grid()
plt.show()
```


​    
![스크린샷 2025-02-22 100733]({{site.url}}\images\2025-02-22-HW4_2\스크린샷 2025-02-22 100733.png)
​    



```python

```
