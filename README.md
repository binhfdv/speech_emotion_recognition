# speech_emotion_recognition

1. Kết quả thực nghiệm trên 2 dạng đặc trưng 1d (Light-GBM, MLP) và 2d (Deep learning).

2. Cây thư mục:
   SourceCode
        
      
    - Feature_1d

            -- cremad
                      --- cremad_mfcc.ipynb
                      --- creamad_melspectrogram.ipynb
                      --- cremad_tempogram.ipynb
                      --- cremad_features_combination.ipynb
                      --- emotion_path.csv
		    -- ravdess
                      --- ravdess_mfcc.ipynb
                      --- ravdess_melspectrogram.ipynb
                      --- ravdess_tempogram.ipynb
                      --- ravdess_features_combination.ipynb
                      --- ravdess_path.csv
              -- ravdess_cremad_features_combination.ipynb

    - Feature_2d

	        -- crema_d_4emo.ipynb
            -- ravdess_4emo.ipynb
            -- done_ravedess_and_crema_d_4emo.ipynb

3. Trong thư mục Feature_1d các file *.ipynb chỉ cần lưu ý đường dẫn tới vị trí các audio (cần download các dataset trước):
    - cremad: `.../cremad/AudioWAV/`. Ví dụ về các path được tạo đến vị trí từng audio trong file emotion_path.csv
    - revdess: `.../ravdess/audio_speech_actors_01-24/`. Ví dụ về các path được tạo đến vị trí từng audio trong file ravdess_path.csv
    - chỉnh sửa đường dẫn nơi lưu model phù hợp.
	
4. Việc tạo file path chỉ cần làm một lần và có thể dùng lại (nếu vị trí audio không đổi) và nên lưu lại các file này tiết kiệm thời gian.

5. Chạy các cell trong *.ipynb để trích xuất đặc trưng và huấn luyện mô hình.