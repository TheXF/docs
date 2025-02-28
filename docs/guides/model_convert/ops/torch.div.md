## torch.div
### [torch.div](https://pytorch.org/docs/stable/generated/torch.div.html?highlight=div#torch.div)
```python
torch.div(input,
          other,
          *,
          rounding_mode=None,
          out=None)
```

### [paddle.divide](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/tensor/math/divide_cn.html#divide)
```python
paddle.divide(x,
              y,
              name=None)
```

其中 Pytorch 相比 Paddle 支持更多其他参数，具体如下：
### 参数差异
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| rounding_mode | -            | 表示舍入模式，PaddlePaddle 无此参数。  |
| out           | -            | 表示输出的 Tensor，PaddlePaddle 无此参数。  |


### 转写示例
#### rounding_mode: 舍入模式
```python
# Pytorch 写法 (rounding_mode 参数设置为"trunc")
x = torch.div([2, 3, 4], [1, 5, 2], rounding_mode='trunc')

# Paddle 写法
x = paddle.divide([2, 3, 4], [1, 5, 2])
x = paddle.trunc(x)

# Pytorch 写法 (rounding_mode 参数设置为"floor")
x = torch.div([2, 3, 4], [1, 5, 2], rounding_mode='trunc')

# Paddle 写法
x = paddle.divide([2, 3, 4], [1, 5, 2])
x = paddle.floor(x)
```

#### out：指定输出
```python
# Pytorch 写法
torch.div([2, 3, 4], [1, 5, 2], out=y)

# Paddle 写法
y = paddle.divide([2, 3, 4], [1, 5, 2])
```
