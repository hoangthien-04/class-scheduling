# Class Scheduling with Genetic Algorithm

Project này cài đặt Genetic Algorithm để lập thời khóa biểu lớp học cho bài Homework 3 - Topic 3.

Notebook chính tập trung vào phần thực nghiệm:

- Sinh dữ liệu đầu vào bằng `random.seed()` để kết quả có thể tái lập.
- Cài đặt các thành phần GA: fitness/penalty, tournament selection, crossover, mutation và elitism.
- Chạy GA để tìm lịch có penalty thấp nhất.
- Vẽ biểu đồ penalty và fitness theo generation.
- Xuất thời khóa biểu cuối cùng ra CSV.

## Files

- `HW3_Topic3_Class_Scheduling_GA.ipynb`: notebook chính, có code, bảng dữ liệu, biểu đồ và kết quả cuối.
- `notebook_code_only.py`: file Python được xuất từ các code cell trong notebook.
- `class_scheduling_ga.py`: phiên bản Python tách hàm đầy đủ hơn.
- `ga_history.csv`: lịch sử chạy GA theo generation.
- `final_class_schedule.csv`: thời khóa biểu cuối cùng.

## How To Run

Chạy notebook trong VS Code hoặc Jupyter:

```powershell
jupyter notebook HW3_Topic3_Class_Scheduling_GA.ipynb
```

Hoặc execute notebook từ terminal:

```powershell
python -m jupyter nbconvert --to notebook --execute --inplace HW3_Topic3_Class_Scheduling_GA.ipynb
```

## Current Result

Lần chạy cuối cùng đã execute thành công:

- Số code cell đã chạy: 12
- Số lỗi khi chạy notebook: 0
- Best penalty cuối cùng: 0
- GA tìm được lịch hợp lệ ở generation 9

Khi `best_penalty = 0`, lịch cuối cùng không còn vi phạm các ràng buộc đã kiểm tra trong notebook.

## Output Files

`ga_history.csv` lưu quá trình cải thiện lời giải:

- `generation`
- `best_penalty`
- `current_best_penalty`
- `avg_penalty`
- `best_fitness`

`final_class_schedule.csv` lưu thời khóa biểu cuối:

- `Section`
- `Course`
- `Session`
- `Professor`
- `Day`
- `Timeslot`
- `Room`
- `Room Size`
- `Class Size`

