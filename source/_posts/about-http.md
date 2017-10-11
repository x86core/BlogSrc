---
title: 关于http协议的说明
tags: http
---
#### 导语：
>了解一下http协议是很有必要的
<hr />
## 1. 请求头格式

| 1    | 2    | ^3    | 4    | 5    |
| ----- | ----- | ------ | ----- |----- |
|1    |2    |3     |4    |5    |
|1    |2    |3     |4    |5    |

 | 排序方法 | 平均情况 | 最好情况 | 最坏情况 | 辅助空间 | 稳定性 |
|:-----|:-----|:-----|:-----|:-----|:-----|
| 冒泡排序 | O(n²) | O(nlogn) | O(n²) | O(1) | 稳定 |
| 简单选择 | O(n²) | O(n²) | O(n²) | O(1) | 稳定 |
| 直接插入 | O(n²) | O(n) | O(n²) | O(1) | 稳定 |
| 希尔排序 | O(nlogn)~O(n²) | O(n^1.3) | O(n²) | O(1) | 不稳定 |
| 堆排序 | O(nlogn) | O(nlogn) | O(nlogn) | O(1) | 不稳定 |
| 归并排序 | O(nlogn) | O(nlogn) | O(nlogn) | O(n) | 不稳定 |
| 快速排序 | O(nlogn) | O(nlogn) | O(n²) | O(nlogn)~O(n) | 不稳定 |

<table style="border-collapse: collapse;border:1px solid red">
    <tr>
        <td>请求方法</td>
        <td>空格</td>
        <td>URL</td>
        <td>空格</td>
        <td>回车、换行</td>
    </tr>
</table>