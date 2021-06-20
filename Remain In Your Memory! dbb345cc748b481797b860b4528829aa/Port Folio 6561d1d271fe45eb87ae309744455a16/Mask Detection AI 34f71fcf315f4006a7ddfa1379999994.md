# Mask Detection AI

생성일: 2021년 6월 15일 오후 11:24
태그: Computer Vision

![Mask%20Detection%20AI%2034f71fcf315f4006a7ddfa1379999994/Mask_Detection_AI.001.jpeg](Mask%20Detection%20AI%2034f71fcf315f4006a7ddfa1379999994/Mask_Detection_AI.001.jpeg)

[Mask Detection AI](Mask%20Detection%20AI%2034f71fcf315f4006a7ddfa1379999994/Mask%20Detection%20AI%20fb08634a9cfd43e0b27dc2e19c4abbc6.csv)

# 개발 목표

백화점 같은 곳을 가면 열을 재는 열화상 카메라가 있다.
이에 영감을 받아 코로나 19사태로 인해 마스크 착용이 의무화 된 이 시점
마스크를 끼지 않은 사람을 Detection하는 AI를 만들어 보고 싶었다.

---

# 개발 내용

기존에 마스크를 인식하는 모델이 있어, 이 모델이 어떤식으로 만들어졌는지 이해하고,
OpenCV를 기반으로 실시간 웹캠을 이용하여 마스크를 쓴 확률을 보여주었다.

---

# 기대효과

사람이 마스크를 안쓴 사람이 있는지 일일이 확인하지 않아도 된다.
이를 응용하여 마스크를 쓰지 않으면 경고음을 울리게 할 수 있다.
또한 우리가 식당에서 밥을 먹으려면 QR코드 인증을 해야하는데,
마스크를 쓰고 있어야만 QR코드가 발급이 될 수 있게 응용 할 수 있다.

---

# 시사점

아쉬운 점은 검정색 Mask의 Accuracy가 좋지 않았던 것이다.
이는 Train Dataset의 문제라고도 할 수 있는데 Mask의 색이 밝은색 계열,
또 cv2.BGR2GRAY를 썼다는 점에서 검은색 마스크 인식률이 좋지 않다고 생각한다.
이는 Mask Dataset을 검정마스크도 낀 것을 추가하거나 색으로 구분하는 것이 
아닌 얼굴이 가려짐을 기준으로 학습을 하면 해결 될 것이라고 생각한다.

---

[CV-JaeHa/Mask_Detection_AI](https://www.github.com/CV-JaeHa/Mask_Detection_AI)