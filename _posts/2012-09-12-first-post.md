---
title: RNN
author: ThanhLeo
layout: post
---
Trong loạt bài về attention mechanism mình có đề cập khá nhiều về mạng RNN. Trong Loạt bài về RNN, mình sẽ giải thích cụ thể hơn về mạng RNN, những biến thể của nó và ứng dụng trong các bài toán cụ thể.

1. RNN là gì?

Mạng nơ-ron hồi quy (RNN - Recurrent Neural Network) là một thuật toán được chú ý rất nhiều trong thời gian gần đây bởi các kết quả tốt thu được trong lĩnh vực xử lý ngôn ngữ tự nhiên. Concept của mạng hoạt động tương tự như việc con người đọc một đoạn text bất kì. Chúng ta không hiểu hết một câu nếu chúng ta không đọc nó từ đầu đến cuối. Cũng như bạn đang đọc bài viết này, bạn hiểu mỗi chữ ở đây dựa vào từ bạn đã hiểu các chữ trước đó. Tức là ta phải làm thế nào để có thể lưu trữ được thông tin như cách mà tư duy hoạt động. Tuy nhiên các mô hình mạng nơ-ron truyền thống thì không thể làm được việc đó, đó có thể coi là một khuyết điểm chính của mạng nơ-ron truyền thống. Và thế là Mạng nơ-ron hồi quy (Recurrent Neural Network) ra đời. Mạng này chứa các vòng lặp bên trong cho phép thông tin có thể lưu lại được.


Nhìn theo góc độ toán học thì mạng RNN được biểu diễn: Mô hình RNN với many to many


Ta thấy lúc này mang xuất hiện 3 ma trận Whh, Wxh, Why. Cả 3 ma trận này sẽ được học trong quá trình trainning mạng RNN. Và được tái sử dụng ở các step của mạng.

Bên cạnh đó mạng RNN cũng được chia thành nhiều mô hình khác nhau như:


2. Vấn đề

Thật không may là với khoảng cách càng lớn dần thì RNN bắt đầu không thể nhớ và học được nữa. 


Ví dụ trong một câu có tầm 20 từ thì h(19) đã khó có thể nhớ được các thông tin của X(0), X(1), ... Việc này ảnh hưởng trực tiếp tới performance của mạng RNN. Và để giải quyết vấn đề này mạng LTSM, GRU đã ra đời. Vì 2 mạng này khá nhiều công thức nên mình giải thích cụ thể ở bài viết tiếp theo.

Bài viết được tham khảo từ: 
https://colah.github.io/posts/2015-08-Understanding-LSTMs/
https://viblo.asia/p/recurrent-neural-networkphan-1-tong-quan-va-ung-dung-jvElaB4m5kw
