# 树型选择 Tree Select

据说 99% 的人分不清它和 Cascader 的区别。

## 演示

```demo
basic
multiple
checkbox
filterable
debug
```

## API

### TreeSelect Props

| 名称 | 类型 | 默认值 | 说明 |
| --- | --- | --- | --- |
| cascade | `boolean` | `false` | 使用 checkbox 进行多选时是否级联 |
| checkable | `boolean` | `false` | 是否使用 checkbox 进行选择 |
| clearable | `boolean` | `false` | 是否可清除 |
| consistent-menu-width | `boolean` | `true` | 是否使菜单宽度和输入框一致，打开会禁用虚拟滚动 |
| default-value | `string \| number \| Array<string \| number> \| null` | `null` | 默认选中的 key |
| default-expand-all | `boolean` | `false` | 默认展开全部 |
| default-expanded-keys | `Array<string \| number>` | `[]` | 默认展开节点的 key |
| disabled | `boolean` | `false` | 是否禁用 |
| expanded-keys | `Array<string \| number>` | `undefined` | 展开节点的 key |
| filterable | `boolean` | `false` | 是否可过滤 |
| filter | `(pattern: string, option: TreeSelectOption) => boolean` | - | 过滤器函数 |
| leaf-only | `boolean` | `false` | 是否开启仅末层树节点可选 |
| max-tag-count | `number \| 'responsive'` | `undefined` | 多选时最多直接显示多少选项，设为 `'responsive'` 会保证最多一行 |
| multiple | `boolean` | `false` | 是否支持多选 |
| options | `TreeSelectOption[]` | `[]` | 选项 |
| placeholder | `string` | `'请选择'` | 占位信息 |
| separator | `string` | `' / '` | 数据分隔符 |
| show-path | `boolean` | `false` | 是否在选择器中显示选项路径 |
| size | `'small' \| 'medium' \| 'large'` | `'medium'` | 组件尺寸 |
| value | `string \| number \| Array<string \| number> \| null>` | `undefined` | 选中的 key |
| virtual-scroll | `boolean` | `true` | 是否开启虚拟滚动 |
| on-blur | `(e: FocusEvent) => void` | `undefined` | Blur 时的回调 |
| on-update:expanded-keys | `(value: Array<string \| number>) => void` | `undefined` | 展开节点更新的回调 |
| on-focus | `(e: FocusEvent) => void` | `undefined` | Focus 时的回调 |
| on-update:value | `(value: string \| number \| Array<string \| number> \| null) => void` | `undefined` | 更新值的回调 |

### TreeSelectOption Properties

| 名称      | 类型                 | 说明                 |
| --------- | -------------------- | -------------------- |
| key       | `string \| number`   | 选项的 key，需要唯一 |
| label     | `string`             | 选项的显示内容       |
| children? | `TreeSelectOption[]` | 节点的子选项         |
| disabled? | `boolean`            | 是否禁用选项         |
