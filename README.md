## 创建ground-truth文件

将xml文件转换成txt文件，文件前缀名和图像一样，信息如下

```html
<class_name> <left> <top> <right> <bottom> [<difficult>]
```

```
tvmonitor 2 10 173 238
book 439 157 556 241
book 437 246 518 351 difficult
pottedplant 272 190 316 259
```

##创建detection-results文件

使用模型跑出结果生成txt文件，文件前缀名和图像一样，信息如下

```
<class_name> <confidence> <left> <top> <right> <bottom>
```

```
tvmonitor 0.471781 0 13 174 244
cup 0.414941 274 226 301 265
book 0.460851 429 219 528 247
chair 0.292345 0 199 88 436
book 0.269833 433 260 506 336
```

## 复制图像

复制图像至images下可显示最终结果，可以不用

## 开始计算

```python
python main.py
```

