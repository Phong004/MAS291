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

- Tung một đồng xu và kết quả là mặt ngửa và tung một xúc xắc cho kết quả là 5.

>P(C) là xác suất tung một đồng xu cho ra mặt ngửa = ${\frac{1}{2}}$  
>P(H) là xác suất tung một xúc xắc cho kết quả là 5 = ${\frac{1}{6}}$  
>${P(C\cup H)=\frac{1}{2}\times \frac{1}{6}=\frac{1}{2}}$  

- Chọn một viên bị từ một hũ và tung một đồng xu cho kết quả là mặt ngửa.
- Chọn một lá 3 từ một bộ bài, đặt nó trở lại, và sau đó chọn một lá át.

>P(3) là xác suất chọn lá 3 từ bộ 52 lá = ${\frac{4}{52}=\frac{1}{13}}$  
>P(A) là xác suất chọn được lá át từ bộ 52 lá = ${\frac{4}{52}=\frac{1}{13}}$  
>${P(3\cup A)=\frac{1}{13}\times\frac{1}{13}=\frac{1}{169}}$  

- Tung một xúc xắc cho kết quả là 4, và sau đó tung ra kết quả 1.

<div align="center">
<img src="Pictures\Independent.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

Hai biến cố được gọi là độc lập khi một trong các mệnh đề tương đương sau thỏa mãn:
    (1) ${P(A|B)=P(A)}$
    (2) ${P(B|A)=P(B)}$
    (3) ${P(A\cap B)=P(A)\times P(B)}$

<div align="center">
<img src="Pictures\MultiIndependent.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>

VD: Nếu một xúc xắc được ném 2 lần, tính xác suất xuất hiện 2 lần 5.  
>${P(A)=\frac{1}{6}}$  
>${P(B)=\frac{1}{6}}$  
>${P(A\cap B)=P(A)\times P(B)=\frac{1}{6}\times\frac{1}{6}=\frac{1}{36}}$  

## 7. Học thuyết Bayes

- Học thuyết Bayes là một định lý cơ bản trong xác suất thống kê, cho phép ta cập nhật xác suất của một giả thuyết khi có thêm thông tin mới.
- Cho hai sự kiện H (giả thuyết/điều kiện) và E(bằng chứng) với ${P(E)\gt 0}$, thì:  
  >${P(H|E)=\frac{P(E|H)\times P(H)}{P(E)}}$  

VD: Trong một khu phố, 90% trẻ em mắc bệnh cúm và 10% mắc bệnh sởi và không có bệnh khác. Xác suất bị phát ban do sởi là 0.95, do cúm là 0.08. Giả sử một đứa trẻ xuất hiện phát ban, tìm xác suất để đứa trẻ đó bị cúm.'

>Gọi F: những đứa trẻ bị cúm  
>M: những đứa trẻ bị sởi  
>R: những đứa trẻ có triệu chứng phát ban  
>${P(F|R)=\frac{P(R|F)\times P(F)}{P(R|M)\times P(M)+P(R|F)\times P(F)}=\frac{0.08\times 0.9}{0.95\times 0.1+0.08\times 0.9}\approx 0.43}$
>${=>P(F|R)=0.43}$

<div align="center">
<img src="Pictures\BayesTheoremK.png" alt="Mutually Exclusive Events for all pairs" style="max-width: 80%; max-height: 500px; height: auto;">
</div>
