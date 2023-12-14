[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/PFJ2jOUW)
# 1. Hello PyTorch, Hello CNN!
Programming Assignment "1. Hello PyTorch, Hello CNN!" for 2023 Summer DeepIntoDeep

**Due Date 2023.07.23**

'D2D' 폴더 전체를 본인의 구글 드라이브에 업로드 한 후에, "1. Hello PyTorch, Hello CNN!.ipynb"를 Colab으로 열어주세요.

Colab 첫번째 Text block의
```FOLDERNAME = None```
을 본인 경로에 맞게 수정하는 것을 잊지 마세요!

## 7.13 수정 - 주의
수업 중간에 말씀해 주셨던 것처럼 AlexNet의 이미지 크기가 227x227이 맞는데 제가 혼동 한 것 같습니다. (저자들이 227이었다 언급했다고 하네요)

첫 번째 Conv Layer가 kernel이 11, stride가 4, padding이 0이 되어야 딱 55 정수가 됩니다. ((227 - 11)/4 + 1 = 55)

하지만 더 찾아보니, 실수가 되더라도 PyTorch가 알아서 값들을 버려준다고 합니다. 혼동을 드려서 죄송합니다!

밑은 제가 혼동했던 CS231n 자료입니다. 그냥 한 번 참고해 주시면 감사하겠습니다.

문제의 경우 이미지 크기를 224 또는 227로 구현해도 상관 없이 고려하겠습니다. **지적해 주셔서 감사합니다!** -지동환-


<img width="698" alt="스크린샷 2023-07-13 오후 6 37 38" src="https://github.com/AIKU-Official/1-hello-pytorch-hello-cnn-hijihyo/assets/35412648/8a83bfa5-7ff3-4fa0-a57d-84935b5d6c86">

## 7.15 수정 - AlexNet Conv Layer 2
AlexNet 재구현 요약 부분에서 Conv Layer 2에 오류가 있어서 바로 잡습니다.

<img width="534" alt="스크린샷 2023-07-15 오후 7 21 36" src="https://github.com/AIKU-Official/1-hello-pytorch-hello-cnn/assets/35412648/73aee2cd-a0fe-412a-ae48-dc0412c4dc18">

Stride가 1, Padding이 2 있는데 오류가 있었습니다. 참고 바랍니다. 혼동을 드려 죄송합니다.
