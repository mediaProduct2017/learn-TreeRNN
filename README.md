# learn-TreeRNN

Tree recursive neural network (TreeRNN)

在自然语言处理方面，Tree recursive neural network是把意义上有修饰或者动作关系的word的vector通过activation function计算得到新的vector（也就是短语phrase所对应的vector），然后再把新的vector和有关系的vector结合起来，得到新的vector，并不断进行下去，理论上，最后一句话、一篇文章也可以用一个多维的vector来描述。

TreeRNN比wholly linked neural network更加实用，但是，相比CNN和RecurretNN，还是有更多的参数（需要首先判断把哪些word归为一类，然后再算此类对应的vector），需要很多的数据来拟合，计算量也很大，大多数时候都没有实用价值。

CNN和RecurretNN有额外的assumption，理论上不够正确，但在目前的数据量和计算能力来说，实用价值更大。就好像生物物理中ligand binding的model中，equilibrium model虽然在理论上不够正确（理论上nonequilibrium model才是正确的），但在有限的数据量和计算能力情况下，实用价值更大，在数据分析中使用的更多。
