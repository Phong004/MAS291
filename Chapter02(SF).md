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
>${P(B)=0.3+0.5+0.1=0.9}$  
>${P(C)=0.1}$  
>${P(A')=1-0.4=0.6}$  
>${P(B')=1-0.9=0.1}$  
>${P(C')=1-0.1=0.9}$  
>${P(A\cap B)=0.3}$  
>${P(A\cup B)=0.4+0.9-0.3=1}$  
>${P(A\cup C)=0.1+0.3+0.1=0.5}$

***Tiên đề của xác suất***

> (1) ${P(S)=1}$  
> (2) ${0\le P(E)\le 1}$  
> (3) Nếu ${A_1, A_2,...}$ là các biến cố rời rạc, ${A_i\cap A_j=\emptyset}$ với ${i\neq j}$ thì: ${P\left(\bigcup_{i=1}^\infty A_i\right) = \sum_{i=1}^\infty P(A_i)}$

## 3. Quy tắc cộng

<div align="center">
<img src="Pictures\ProbabilityUnion.png" alt="Probability Union Addition" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

VD: Một lớp có 28 sinh viên, 12 học tiếng Nhật, 15 học tiếng Anh và 8 sinh viên học cả hai môn. Một sinh viên được chọn ngẫu nhiên, tính xác suất để chọn ra những sinh viên học tiếng Nhật hoặc tiếng Anh.

>- Gọi A là tập các sinh viên học tiếng Nhật có 12 phần tử.
>- Gọi B là tập các sinh viên học tiếng Anh có 15 phần tử.
>- Xác suất chọn ra sinh viên học tiếng Nhật hoặc tiếng Anh: ${P(A\cup B)=P(A)+P(B)-P(A\cap B)=\frac{12}{28}+\frac{15}{28}-\frac{8}{28}=\frac{19}{28}}$

***Mutually Exclusive Events*** là các sự kiện không thể diễn ra đồng thời trong một phép thử hoặc trong một tình huống. Nói cách khác, nếu sự kiện A xảy ra thì sự kiện B sẽ không xảy ra và ngược lại. Thuật ngữ tiếng Việt là các biến cố loại trừ lẫn nhau.

<div align="center">
<img src="Pictures\MutuallyExclusiveEventsAddition.png" alt="Mutually Exclusive Events" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

<div align="center">
<img src="Pictures\MutuallyExclusiveEventsAddition2.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

VD: Cho X ký hiệu độ pH của một mẫu thử. Biến cố X lớn hơn 6.5 nhưng nhỏ hơn hoặc bằng 7.8. Xác suất này là tổng của tất cả các bộ biến cố loại trừ lẫn nhau với phép hợp bằng giới hạn tương tự cho X.

<div align="center">
<img src="Pictures\Example2-3.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

Khoảng cách của các biến cố càng nhỏ thì kết quả càng tốt.

<div align="center">
<img src="Pictures\AdditionRules.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

## 4. Xác suất có điều kiện

- Xác suất có điều kiện là xác suất của một sự kiện B xảy ra khi sự kiện A đã xảy ra (${A\neq B}$)
- Tính xác suất sự kiện B xảy ra khi đã xảy ra sự kiện A chính là xác suất của ${B\cap A}$ với không gian mẫu giảm xuống còn bằng A (ký hiệu: P(B|A))

> ${P(B|A) = \frac{P(A\cap B)}{P(A)}}$  
> ${P(A\cap B) = P(B|A) \times P(A)}$

<div align="center">
<img src="Pictures\ConditionalProbabilityFormula.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

VD: Trong một lớp học, 35% sinh viên nghiên cứu khoa học và lịch sử. 65% nghiên cứu khoa học. Tính xác suất của sinh viên nghiên cứu lịch sử *sau khi đã nghiên cứu khoa học*?

>- Sinh viên nghiên cứu khoa học là S
>- Sinh viên nghiên cứu lịch sử là H  
>${P(S\cup H)=0.35}$  
>${P(S)=0.65}$  
>${=> P(H|S)=\frac{P(H\cap S)}{P(S)}=\frac{0.35}{0.65}=0.53}$

## 5. Quy tắc nhân và tổng xác suất

### Quy tắc nhân

<div align="center">
<img src="Pictures\MultiplicationRule.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

**Giải thích công thức:**
    ${P(A|B)=\frac{P(A\cap B)}{P(B)} => P(A\cap B)=P(A|B)\times P(B)}$  
    ${P(B|A)=\frac{P(A\cap B)}{P(A)} => P(A\cap B=P(B|A)\times P(A))}$

VD: Một sọt chứa 12 banh hồng và 6 banh xanh. Không hoàn lại, 2 trái được lấy ra lần lượt từng quả. Xác suất để cả 2 quả banh được rút ra cùng là màu hồng?

>- A là xác suất rút ra quả banh màu hồng lần đầu tiên  
>- B là xác suất rút ra quả banh màu hồng lần thứ hai  
>${P(A)=\frac{12}{18}, P(B|A)=\frac{11}{17}}$  
>${=>P(A\cap B)=P(A)\times P(B|A)=\frac{12}{18}\times \frac{11}{17}=\frac{132}{306}}$

### Tổng xác suất (2 biến cố)

- Cho không gian mẫu S có các không gian con: A, A', B, B giao với cả không gian A, và A'. Khi này, ${P(B)=P(B\cap A)+P(B\cap A')}$

<div align="center">
<img src="Pictures\TotalProbabilityRule.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

### Tổng xác suất (đa biến cố)

<div align="center">
<img src="Pictures\TotalProbabilityRule2.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

VD: Giả sử xác suất sản xuất các linh kiện bán dẫn có độ thất bại được đo như sau:

<div align="center">
<img src="Pictures\Example2-5-1.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

## 6. Sự độc lập

**Một số các ví dụ về các biến cố độc lập:**
- 