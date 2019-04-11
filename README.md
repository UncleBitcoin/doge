# Doge
### 尝试从dogetip研究够狗狗币分叉  
建立代码库


#### fork 狗狗币代码
#### fork Dogetip代码
将两者对比后结合上传

# 编译结合后的代买 客户端
## 安装系统依赖

    sudo apt install build-essential libtool autotools-dev automake pkg-config bsdmainutils curl
编译Win钱包需要
    
    sudo apt install g++-mingw-w64-i686 mingw-w64-i686-dev g++-mingw-w64-x86-64 mingw-w64-x86-64-dev nsis
编译Linux钱包需要
    
    sudo apt install gcc-4.8-multilib g++-4.8-multilib
# 第二步 同步比特币代码
0.12版
    
    https://git.ustclug.org/SilentYang/Bitcoin-Dp
0.14版
    
    https://git.ustclug.org/altcoin/bitcoin
# 第三步 开始编译
## 处理编译环境

    cd depends
编译Win钱包需要
    
    make HOST=i686-w64-mingw32                      #32位
    make HOST=x86_64-w64-mingw32                    #64位
编译Linux钱包需要
    
    make HOST=i686-pc-linux-gnu                     #32位
    make HOST=x86_64-pc-linux-gnu                   #64位
## 配置编译好的编译器

    cd ..
    ./autogen.sh
以下指令排他，一次只能编译一种系统的钱包。

    ./configure --prefix=`pwd`/depends/i686-w64-mingw32
    ./configure --prefix=`pwd`/depends/x86_64-w64-mingw32
    ./configure --prefix=`pwd`/depends/i686-pc-linux-gnu
    ./configure --prefix=`pwd`/depends/x86_64-pc-linux-gnu
## 开始编译
    
    make

编译Win版本可以通过以下指令生成安装包

    make deploy.



----------------------------------------------------------------------------------------------------------------------------------------

# Mining Pool 矿池  
1. http://pool.dogetip.org/     
2. http://172.105.240.230


----------------------------------------------------------------------------------------------------------------------------------------

# Features 特色

Total Supply: 118,500,000,000 (Max)  总量1185亿；  
Lightning fast transaction  闪电般的交易速度;      
Extremely low transaction fee  极低的交易费用;               
Smart contract integrated(developing...)   加入智能合约(开发中);     
Zero-knowledge Proof private transaction(developing...)   零知识证明隐私交易(开发中);       

# Specification 参数
Algorithm: Scrypt (AuxPoW)  算法：Scrypt (辅助PoW挖矿);    
Block Time: 60 Seconds  区块时间：60秒;     
Difficulty Retarget: Digishield  难度调整：Digishield;    
Premined 300,000,000  预挖：3亿;    

# Block Reward 区块奖励 
Block 2,123,456 - 2,199,999: 10,000 DTP  区块高度2,123,456 - 2,199,999: 10,000 DTP奖励;    
Block 2,200,000 - 2,299,999: 80,000 DTP  区块高度Block 2,200,000 - 2,299,999: 80,000 DTP奖励;    
Block 2,400,000 + :  reduce 20%  at every 100,000 Block  区块高度Block 2,400,000 + :  每100,000区块高度减产20%;    



# Vision 愿景
Inspired by Dogecoin, we are going to create a Blockchain spirit currency for tipping  and donating.
We are planning to use 300,000,000 DTP to developing and marketing.   
受狗狗币启发，为打赏和捐献创造忠于区块链精神的加密货币.  
我们将会使用3亿DTP来开发Dogetip和市场推广.  


# Link 链接
Twitter推特: https://twitter.com/Dogetip_org    
Bitcointalk: https://bitcointalk.org/index.php?topic=2933956.msg30143128#msg30143128
