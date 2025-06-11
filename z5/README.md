# 9.RNN

## 3.数据预处理验证

<img width="760" alt="91610388262da257e439494e595ed33" src="https://github.com/user-attachments/assets/b1116764-d0e7-44b9-8b5d-58eb61f34652" />




## 4.模型结构验证
<img width="740" alt="479ac7eba37b657e4fa80789c53494d" src="https://github.com/user-attachments/assets/f4606489-a525-4fc1-862d-4eaf64b36b3a" />



## 5.RNN序列处理验证
<img width="750" alt="414d34dc7862293ed9a4bb3b5c6d15b" src="https://github.com/user-attachments/assets/96708d3c-d8de-4330-b7dd-e06d6c1b97e3" />


## 6.模型性能评估

## 7.推理能力验证
<img width="559" alt="208268297bc310d48a0791bc19467ad" src="https://github.com/user-attachments/assets/1148405a-efa9-4ae7-a0fa-57ee9570ff4d" />

# 10.RNN 



### 无条件姓氏生成

<img width="722" alt="67a945a777c10531532aa26582c32c3" src="https://github.com/user-attachments/assets/2bec3121-7148-4347-97d7-8d880945825a" />


### 有条件姓氏生成
<img width="694" alt="8acac407f5906fc6d3d6f1871bf750b" src="https://github.com/user-attachments/assets/c9f53dc1-a20d-4dfb-b375-2226bab70fb3" />



## 4、**回答问题**

① 两个模型的核心差异体现在什么机制上？  **B**

A. 字符编码方式不同

B. 是否考虑国家信息作为生成条件

C. RNN单元类型不同（GRU/LSTM）

D. 损失函数计算方式不同

② 在条件生成模型（Model2_Conditioned_Surname_Generation）中，国家信息通过什么方式影响生成过程？  **B**

A. 作为额外的输入特征拼接

B. 作为GRU的初始隐藏状态

C. 作为注意力机制的key

D. 作为输出层的偏置项

③ 文件2中新增的nation_emb层的主要作用是：  **B**

self.nation_emb = nn.Embedding(num_nationalities, rnn_hidden_size)

A. 将字符索引映射为稠密向量

B. 将国家标签转换为隐藏状态初始化向量

C. 生成姓氏的长度控制参数

D. 计算交叉熵损失的辅助参数

④ 对比两个文件的sample_from_model函数，文件2新增了哪个关键参数？  **B**

A. temperature

B. nationalities

C. device

D. max_length
