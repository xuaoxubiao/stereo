# 2018_Q3_软件开发工程师
    * 应聘者：徐彪 
    * 联系电话：13258259528
    * 电子邮件：xubiao920627@163.com
## 设计思路
      1、定义一个二维数组，并将行和列都为奇数的下标值设为0表示路，其余值均为1表示墙；
      2、输入连通区域后将坐标按顺序保存在一维向量中，并计算为渲染网格的对应坐标
      3、循环遍历向量，将二维数组中对应下标的元素值改为0，其余不变；
      4、渲染网格，遍历二维数组，将值为0的对应元素输出为"[R] ",值为1的对应元素输出为"[W] "

### 如何运行
      启动vs工程文件，按照要求格式输入道路网格和连通区域坐标。
      注意：
      1、道路网格输入格式为"M N"(数字中间用空格隔开，用回车表示结束)
      2、连通区域格式为"x1,x2 y1,y2;x3,x4 y3,y4"(同一坐标行和列之间用","隔开，同一组坐标中间用空格隔开，一组坐标结束后用";"隔开，最后一组结束后用回车表示结束）
      输入示例：
      3 3
      0,1 0,2;0,0 1,0;0,1 1,1;0,2 1,2;1,0 1,1;1,1 1,2;1,1 2,1;1,2 2,2;2,0 2,1

#### 运行结果
      Please input the size of Maze(input value for m,n):3 3
      Please input the connected coordinate：0,1 0,2;0,0 1,0;0,1 1,1;0,2 1,2;1,0 1,1;1,1 1,2;1,1 2,1;1,2 2,2;2,0 2,1
      [W] [W] [W] [W] [W] [W] [W]
      [W] [R] [W] [R] [R] [R] [W]
      [W] [R] [W] [R] [W] [R] [W]
      [W] [R] [R] [R] [R] [R] [W]
      [W] [W] [W] [R] [W] [R] [W]
      [W] [R] [R] [R] [W] [R] [W]
      [W] [W] [W] [W] [W] [W] [W]
