# Speech to Speech Translation(S2ST) with Diffusion Model


* 기존 S2ST 모델은 ASR -> MT -> TTS로 이루어진 Cascaded S2ST 형태이며, 이는 학습 시에 많은 데이터와 시간 그리고 컴퓨팅 소소를 요구함.
* 이를 완화하기 위해 본 연구에서는 E2E 방식의 S2ST 기술의 연구를 진행함.
* 최근 Diffusion 모델은 생성 AI 분야에서 두각을 드러내고 있음. 기존 생성 AI 모델 GAN과 비교하여 명시적으로 확률적 모델링을 기반으로 학습하기에 Mode Collapse의 빈도가 적으며, MultiModal 데이터 기반의 생성에서 경쟁력이 있음.
* 본 연구에서는 Diffusion Model을 활용하여 입력 화자의 음성 특징을 보존한 채 target 언어로 변환된 음성 생성을 생성하는 S2ST 모델을 설계하려 함. 


---



DDPM 및 [SDE Diffusion Model](https://colab.research.google.com/drive/120kYYBOVa1i0TD85RjlEkFjaWDxSFUx3?usp=sharing#scrollTo=8PPsLx4dGCGa)의 튜토리얼 코드를 기반으로 [Classifier-Guided Diffusion Model](https://github.com/openai/guided-diffusion/tree/main), [Classifier-free Diffusion Model](https://arxiv.org/abs/2207.12598)의 offical code와 논문을 참조하여 Speech Enhancement PoC 수행 




