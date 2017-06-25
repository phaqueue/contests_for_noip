### A
  <br />这是一道贪心，顺序什么的并不重要。因此本着贪到贪无可贪的原则，我们只需输出所有的0和1的个数再减一减就可以A掉了
### B
  <br />此题有o(n)的标程(http://paste.ubuntu.com/11788578/)
  <br />不过作为一只蒟蒻，本渣只打出了n^2程序
  <br />思路大致如下
  <br />转一遍，检验一遍，如果转完n次仍不能成功，那就没有什么价值继续了，输出’NO'
### C
  如果不是从一开始连着套的套娃，总是要拆开来的，多分几份反而是方便了，有n份就少开了n个，合并共需m-1次。有1-k连的情况，拆分合并均省k次，综上所述，共需2m+1-n-2l次
### D
  每个岛(l,r)，应该尽量找大于等于l，并且小于等于r，跟r相差最小的，那么可以对岛进行排序，然后维护一个set，用来找离r最近的是哪座桥。
### E
  首先离散化，我是对x坐标离散的，然后维护一个左边界限和上边界线，每次之需要查询，然后进行更新，更新的时候要注意，是更新这个点和他能走到的那个格子的x坐标之间的副对角线上的点