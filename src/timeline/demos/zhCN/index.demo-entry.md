# 时间线 Timeline

这个世界有两个纬度：时间、事件。

## 演示

```demo
basic
size
item-placement
horizontal
```

## Props

### Timeline Props

| 名称           | 类型                  | 默认值     | 说明   |
| -------------- | --------------------- | ---------- | ------ |
| horizontal     | `boolean`             | `'false'`  | 水平的 |
| item-placement | `'left' \| 'right'`   | `'left'`   | 方向   |
| size           | `'medium' \| 'large'` | `'medium'` | 大小   |

### Timeline Item Props

| 名称 | 类型 | 默认值 | 说明 |
| --- | --- | --- | --- |
| content | `string` | `undefined` | 选项内容 |
| time | `string` | `undefined` | 选项时间 |
| title | `string` | `undefined` | 选项标题 |
| type | `'default' \| 'success' \| 'info' \| 'warning' \| 'error'` | `'default'` | 选项类型 |

## Slots

### Timeline Slots

| 名称    | 参数 | 说明       |
| ------- | ---- | ---------- |
| default | `()` | 时间线内容 |

### Timeline Item Slots

| 名称    | 参数 | 说明               |
| ------- | ---- | ------------------ |
| default | `()` | 时间线选项内容     |
| footer  | `()` | 时间线选项底部内容 |
| header  | `()` | 时间线选项头部内容 |
