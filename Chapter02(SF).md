# Chương 2: Xác xuất

## 1. Giới thiệu

- Sử dụng để định lượng xác xuất hoặc khả năng xảy ra của một sự kiện.
- Được sử dụng để biểu diễn rủi ro hoặc bất định trong một các ứng dụng kỹ thuật.
- Có thể diễn giải là mức độ tin tưởng hoặc tần suất tương đối.

## 2. Sự diễn giải của xác suất

***Thí nghiệm ngẫu nhiên***
> Một thí nghiệm có thể có nhiều kết quả đầu ra khác nhau, thậm chí được thực hiện nhiều lần tương tự được gọi là **thí nghiệm ngẫu nhiên**

***Không gian mẫu***
> Tập các đầu ra có thể xảy ra của một **thí nghiệm ngẫu nhiên** được gọi là **không gian mẫu** của thí nghiệm.

***Biến cố***
> Một **biến cố** là một tập con của không gian mẫu của một thí nghiệm ngẫu nhiên.

***Các kết quả có cùng xác suất***
> Bất cứ khi nào một không gian mẫu có N kết quả có thể xảy ra có xác suất như nhau, xác suất của mỗi kết quả là ${\frac{1}{N}}$

***Xác suất của một biến cố***
> Cho một không gian mẫu rời rạc, xác suất của một biến cố E - P(E), bằng tổng xác suất của các kết quả của E.

VD: Một thí nghiệm ngẫu nhiên có kết quả trong một trong các đầu ra {a, b, c, d} với xác suất 0.1, 0.3, 0.5, 0.1 tương ứng. ${A=\\{a,b\\}, B=\\{b,c,d\\}, C=\\{d\\}}$

>${P(A)=0.1+0.3=0.4}$
>
>${P(B)=0.3+0.5+0.1=0.9}$
>
>${P(C)=0.1}$
>
>${P(A')=1-0.4=0.6}$
>
>${P(B')=1-0.9=0.1}$
>
>${P(C')=1-0.1=0.9}$
>
>${P(A\cap B)=0.3}$
>
>${P(A\cup B)=0.4+0.9-0.3=1}$
>
>${P(A\cup C)=0.1+0.3+0.1=0.5}$

***Tiên đề của xác suất***

> (1) ${P(S)=1}$
>
> (2) ${0\le P(E)\le 1}$
>
> (3) Nếu ${A_1, A_2,...}$ là các biến cố rời rạc, ${A_i\cap A_j=\emptyset}$ với ${i\neq j}$ thì: ${P\left(\bigcup_{i=1}^\infty A_i\right) = \sum_{i=1}^\infty P(A_i)}$

## 3. Quy tắc cộng

<div align="center">
<img src="Pictures\ProbabilityUnion.png" alt="Probability Union Addition" style="max-width: 80%; max-height: 500px; height: auto;">
</div>


2.4 Condition Probability
- ${P(B|A) = P(A\cap B) / P(A)}$
- ${P(A\cap B) = P(B|A) \times P(A)}$

