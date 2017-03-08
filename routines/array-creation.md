### 全0和全1的数据块

empty\( **`shape`**,      dtype,  order \)           创建一块空数据，没有初始化工作，节省时间

empty\_like\( **`a`**,      dtype, order, subok \)  创建一块空数据，它的shape和a.shape一样。

eye\( **`N`**,     M, k, dtype_ _\) 2D单位矩阵，对角线全1，其余为0

identity\( **`n`**,    dtype\) 单位矩阵

ones\( **`shape`**,  dtype, order \)            全1数据块

ones\_like\( **`a`**,  dtype, order, subok \) 全1数据块

zeros\( **`shape`**,  dtype, order \) 全0数据块

zeros\_like\( **`a`**,  dtype, order, subok \) 全0数据块

full\( **`shape, fill_value`**, dtype, order \) 全 fill-value 的数据块

fulllike\( **`a, fill_value`**,  dtype, order, subok \) 全 fill-value 的数据块

