<!-- Banner -->
<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: none;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<h1 align="center"><b>TRÍ TUỆ NHÂN TẠO</b></h>

## THÀNH VIÊN NHÓM

| STT    | MSSV          | Họ và Tên              | Github                                               | Email                   |
| ------ |:-------------:| ----------------------:|-----------------------------------------------------:|-------------------------:
| 1      | 20521597      | Đinh Nhật Minh         |https://github.com/Banhkun	                        |20521597@gm.uit.edu.vn   |
| 2      | 20520731      | Trần Thị Mỹ Quyên |https://github.com/AzaleaBrowns |20520731@gm.uit.edu.vn   |
| 3      | 20521424      | Văn Nguyễn Ngọc Huyền |https://github.com/ngochuynnuit |20521424@gm.uit.edu.vn   |
|       | 20521444      | Dương Thành Bảo Khanh          |                      https://github.com/cptdtbk                      |20521444@gm.uit.edu.vn   |




## GIỚI THIỆU MÔN HỌC

-   **Tên môn học:** Trí tuệ nhân tạo 
-   **Mã môn học:** CS116
-   **Mã lớp:** CS116.M21
-   **Năm học:** HK2 (2021 - 2022)
-   **Giảng viên**: TS.Lương Ngọc 

## ĐỒ ÁN CUỐI KÌ

-   **Tên đề tài**: ABSTRACTIVE QUESTION
SUMMARIZATION WITH
QUESTION-AWARE SEMANTIC REWARDS

-   **Giới thiệu**
   -Tóm tắt văn bản (Summarization) là tác vụ cô đọng một đoạn văn bản thành phiên bản gắn gọn hơn nhưng vẫn bảo toàn các thông tin cần thiết và nội dung chính. Vì tóm tắt văn bản thủ công rất tốn kém thời gian và công sức, việc tự động hóa tác vụ này đang ngày càng phát triển và tạo động lực mạnh mẽ cho các nghiên cứu học thuật.
    -  “Tóm tắt trừu tượng” (Abstractive summarization) là nhóm phương pháp ứng dụng kỹ thuật Xử lý ngôn ngữ tự nhiên (NLP) tạo ra các văn bản tóm tắt tối ưu, có thể chứa các từ không được trình bày tài liệu gốc. Có thể thấy, văn bản tóm tắt sẽ tập trung truyền tải các thông tin quan trọng nhất, tức yêu cầu khả năng diễn đạt lại văn bản và kết hợp thông tin, như cách con người tóm tắt văn bản. Do đó, một văn bản trừu tượng đạt chuẩn cần chứa đủ thông tin cốt lõi, đồng thời đạt được sự trôi chảy, tự nhiên về mặt ngôn ngữ.
- Trong đồ án , chúng tôi lựa chọn bài toán Tóm tắt câu hỏi trừu tượng (Abstractive Question Summarization) trong lĩnh vực sức khoẻ, y tế, cụ thể là câu hỏi y tế từ người dùng (Consumer Health Questions - CHQ), nhằm đơn giản hoá các câu hỏi truy vấn dài dòng và nhiều thông tin dư thừa, hỗ trợ phản hồi người dùng đáp án nhanh chóng và hiệu quả.

-   **Hướng dẫn cài đặt**
-   # Reinforcement Learning for Abstractive Question Summarization with Question-aware Semantic Rewards



The code requires **Python 3** and please install the Python dependencies with the command:
```bash
pip install -r requirements.txt
```

The original MeQSum dataset is available [here](https://github.com/abachaa/MeQSum).


### Running the code 
1. Please make sure to download the pre-trained question-type identification and question-focus recognition models from [here](https://drive.google.com/drive/folders/1ePtuMPR20rZSgZbarSnno4-sqazLJVn0?usp=sharing) and 
    place it in the current directory.

2. Fine tune ProphetNet model on MeQSum dataset

    Follow the instrcution from transformers repo.
    https://github.com/huggingface/transformers/tree/v4.1.1/examples/seq2seq
 

3. Train MLE + RL Model
    ```
    python main.py --train_mode rl --trained_model_path /path/to/the/fine-tuned/prophetnet/model
    ```

4. Test Model
    ```
    python main.py --model test --trained_model_path /path/to/the/saved/model

    ```


## Reference

If you are using this code for your reseach work then please cite our paper:
```
@inproceedings{yadav-etal-2021-reinforcement,
    title = "Reinforcement Learning for Abstractive Question Summarization with Question-aware Semantic Rewards",
    author = "Yadav, Shweta  and
      Gupta, Deepak  and
      Ben Abacha, Asma  and
      Demner-Fushman, Dina",
    booktitle = "Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing (Volume 2: Short Papers)",
    month = aug,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.acl-short.33",
    doi = "10.18653/v1/2021.acl-short.33",
    pages = "249--255"
    }
```

    ```bash
      git clone https://github.com/Banhkun/CS106---Question-Summarizing
      cd Inpainting-with-seam-carving
    ```
    To emulate our project, following our instruction in jupyter notebook:
    <h3 align="left">
        <a href="https://karhdo.github.io/CS231.M21/">DEMO</a>
    </h3>
    <img align="center" src="./demo.gif">
