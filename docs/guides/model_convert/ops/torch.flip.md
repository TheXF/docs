## torch.flip
### [torch.flip](https://pytorch.org/docs/stable/generated/torch.flip.html?highlight=flip#torch.flip)

```python
torch.flip(input,
           dims)
```

### [paddle.flip](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/flip_cn.html#flip)

```python
paddle.flip(x,
            axis,
            name=None)
```

两者功能一致且参数用法一致，仅参数名不同，具体如下：
### 参数差异
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| input         | x            | 输入的 Tensor。                   |
| dims          | axis         | 需要翻转的轴。                     |
