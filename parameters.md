## 物理模型：位置，电荷，自旋等

### geometry.in 标签
1. atom
  > Usage: atom x y z species_name
  > 作用：指定原子初始位置和类型
  > 注意：x y z 单位为埃，species_name需要是control.in中已给出的原子

1. atom_frac
 > Usage: atom_frac n<sub>1</sub>  n<sub>2</sub>  n<sub>3</sub> species_name
 > 作用：使用分数坐标指定原子初始位置和类型
 > 注意： n<sub>i</sub>是晶格向量的系数，species_name需要是control.in中已给出的原子，分数坐标仅在周期计算中生效

1. lattice_vector
>Usage: lattice_vector x y z
>作用：为周期性结构指定晶格向量
>注意： x y z为单位为埃的实数，表征晶胞向量的长度和方向，*如果指定三个晶格向量，aims自动假定三个方向的边界条件，三个向量的顺序很重要，因为，control.in中给出的k空间划分依赖于晶格向量的顺序。*

###control.in标签

1. charge
> Usage: charge q
> 作用： 指定一个系统总体电荷（可选）
> 注意： 
