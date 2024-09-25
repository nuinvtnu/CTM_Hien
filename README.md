Chương trình demo Đề tài Luận văn tốt nghiệp "**Mô hình phân tích dự đoán vị trí protein Arabidopsis Ubiquitination sử dụng phương pháp chắt lọc tri thức**"
(Học viên: Cù Thị Mai Hiên; GVHD: TS. Nguyễn Văn Núi)

----
**Cấu hình**
Google Colab.
  Library: Keras, Tensorflow, Sklearn
  Input: format: .csv ; windowsize: 31
Prediction: step-by-step as followings:

----
  Step 1: Data collection and pre-processing
  
  Step 2: Extract fragments using window size of 31
  
  Step 3: Removing redundant and homologous data using CD-HIT
 
  Step 4: Word separating using 1-gram

  Step 5: Training the model on CSV files
 
 ----
    Build teacher model:
    Train teacher model with teacher dataset and save this model: teacher_KD2.h5
    Evaluate model using 5-fold cross-validation:
    Load model teacher_KD2.h5
    Define Knowledge distillation model
    Train model Knowledge distillation with 5-fold cross validation
    Save model the best of Knowledge distillation model: KD2_1gram.h5
