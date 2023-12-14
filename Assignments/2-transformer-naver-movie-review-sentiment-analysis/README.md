# 2. Transformer, Naver Movie Review Sentiment Analysis
Programming Assignment "2. Transformer, Naver Movie Review Sentiment Analysis" for 2023 Summer DeepIntoDeep


Due date: 2023.08.04

"2. Transformer, Naver Movie Reive Sentiment Analysis" 파일을 코랩에서 열어주시고 dataset.zip 파일을 압축 풀어서 구글 드라이브에 업로드 해주세요!


업로드한 경로를 Google Drive Mount 이후에 data_dir 변수에 올바르게 설정해주세요!

# 7.26 수정


TF_Encoder Class 구현에서 __init__ 부분에 수정사항이 있습니다!

과제를 아직 시작하지 않으신 분의 경우에는 새로 업로드한 파일 이용해주시면 되고 이미 시작하신 분의 경우

__init__에서 

"self.enc_blocks = TF_Encoder_Block(d_model, d_ff, num_head, dropout)"

부분을

"self.enc_blocks = nn.ModuleList([TF_Encoder_Block(d_model, d_ff, num_head, dropout) for _ in range(num_layer)])"

으로 수정해주시면 되겠습니다!
