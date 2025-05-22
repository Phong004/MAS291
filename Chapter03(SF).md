# Chapter 03: Biến ngẫu nhiên rời rạc và phân phối xác suất

## I. Biến rời rạc ngẫu nhiên

- Một biến rời rạc ngẫu nhiên là một biến ngẫu nhiên có tập xác định có hạn (hoặc vô hạn đếm được).

VD1: Tung 1 xung xắc 2 lần, số lần xuất hiện mặt 5:  
>${\Omega=\\{55,5N,N5,NN\\}}$  
>X(5s)={0,1,2}

VD2: Tung 1 đồng xu 3 lần, số lần xuất hiện mặt ngửa?
>${\Omega=\\{HHH,HHT,HTH,HTT,THH,THT,TTH,TTT\\}}$  
>X(heads)={3,2,1,0}

## II. Phân phối xác suất và hàm khối xác suất

***Phân phối xác suất***

- Một phân phối xác suất của một biến ngẫu nhiên X là một xác suất liên quan với các giá trị khả dĩ của X.

<div align="center">
<img src="Pictures\PDExample.png" alt="Probability Union Addition" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

***Hàm khối xác suất***

- Cho một biến ngẫu nhiên rời rạc X với các giá trị khả dĩ ${x_1, x_2, ..., x_n}$, một hàm khối xác suất là một hàm:

>(1) ${f(x_1)=P(X=x_i)}$  
>(2) ${f(x_i)\ge 0}$  
>(3) ${\sum_{i=1}^{n}f(x_i)=1}$

<div align="center">
<img src="Pictures\PMFExample.png" alt="Probability Union Addition" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

VD3: Có một khả năng một bit được truyền qua một kênh truyền dẫn số bị lỗi. Cho X bằng số bit bị lỗi trong 4 bit được truyền. Các giá trị khả dĩ của X là {0, 1, 2, 3, 4}. Giả sử rằng xác suất là:  
    ${P(X=0)=0.6561}$   ${P(X=1)=0.2916}$  
    ${P(X=2)=0.0486}$   ${P(X=3)=0.0036}$
    ${P(X=4)=0.0001}$

<div align="center">
<img src="Pictures\PMFNextExp.png" alt="Probability Union Addition" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

## III. Hàm 


## VI. Phân phối nhị thức

- TÍnh xác suất x lần xảy ra trong n phép thử:
    n: số phép thử
    s: số lần thành công
    p: xác suất thành công.\

## VII. Phân phố hình học và phân phối nhị thức âm

### 1. Phân phối hình học

- Là tính xác suất đến số lần thử đến lần thành công đầu tiên

>${f(x)=P(X=x)=(1-p)^{x-1}\times p, x\gt 1}$  
>${u=E(X)=\frac{1}{p}}$  
>${\sigma^2=V(X)=\frac{1-p}{p^2}}$


### 2. Phân phối nhị thức âm

- Là tính xác suất xảy ra đến r lần thử thành công xảy ra

>${f(x)=P(X=x)=C^{r-1}_{n-1}\times (1-p)^(x-r)\times(1-p)^{n-x}, x\gt 0}$  
>${u=E(X)=n\times p}$  
>${\sigma^2=V(X)=n\times p\times (1-p)}$ 

### 3. Phân phối siêu bội

<div align="center">
<img src="Pictures\HyperDistribution.png" alt="Probability Union Addition" style="max-width: 80%; max-height: 500px; height: auto;">
</div>
