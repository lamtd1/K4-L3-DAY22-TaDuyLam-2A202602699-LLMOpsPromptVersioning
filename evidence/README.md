# Phân tích so sánh Prompt V1 vs V2

## Kết quả RAGAS

| Metrics | V1 | V2 | Chênh lệch | Nhận xét |
|---------|----|----|-----------|---------|
| **Faithfulness** | 0.991 | 0.9849 | -0.0061 | V1 cao hơn — output V1 trung thực hơn với context |
| **Answer Relevancy** | 0.6465 | 0.6644 | +0.0179 | V2 cao hơn — câu trả lời V2 liên quan hơn đến câu hỏi |
| **Context Recall** | 1.0 | 1.0 | 0 | Cân bằng — cả 2 đều truy xuất được tất cả document liên quan |
| **Context Precision** | 0.9450 | 0.9450 | 0 | Cân bằng — cả 2 đều chọn đúng document |

## Kết luận

**V1 vs V2: Cân bằng — target met ✅**

- **V1 ưu điểm:** Trung thực hơn (faithfulness cao 0.7%), ít bị hallucination
- **V2 ưu điểm:** Liên quan hơn (answer_relevancy tăng 1.8%), trả lời sát vấn đề hơn

**Lựa chọn:** Nên chọn **V2** vì sự cải thiện về answer relevancy (người dùng sẽ cảm thấy câu trả lời sát với câu hỏi hơn), với faithfulness vẫn giữ ở mức rất cao (0.9849). Sự trade-off này phục vụ tốt hơn trải nghiệm người dùng.


