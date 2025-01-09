# Speech to Speech Translation(S2ST) with Diffusion Model




<div align="center">
 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/S2ST_abs.png width = "80%" height = "80%">

**S2ST Model**

</div>


* 기존 S2ST 모델은 ASR-> MT->TTS로 이루어진 Cascaded S2ST 형태, 이는 오류 전파의 문제와 더불어 학습에 많은 데이터와 시간 그리고 컴퓨팅 소스를 요구함.
* 해당 문제들을 완화하기 위해 본 연구에서는 E2E 방식의 S2ST 기술의 연구를 진행.
* Diffusion Model은 생성 AI 분야에서 두각을 보임. 기존 생성 AI 모델 GAN과 비교하여 명시적으로 확률적 모델링을 기반으로 학습하기에 Mode Collapse의 빈도가 적으며, MultiModal 데이터 기반의 생성에서 경쟁력이 있음.
* 본 연구에서는 Diffusion Model을 활용하여 입력 화자의 음성 특징을 보존한 채 target 언어로 변환된 음성 생성을 생성하는 S2ST 모델 설계를 시도. 

</br>





DDPM 및 [SDE Diffusion Model](https://colab.research.google.com/drive/120kYYBOVa1i0TD85RjlEkFjaWDxSFUx3?usp=sharing#scrollTo=8PPsLx4dGCGa)의 튜토리얼 코드를 기반으로 [Classifier-Guided Diffusion Model](https://github.com/openai/guided-diffusion/tree/main), [Classifier-free Diffusion Model](https://arxiv.org/abs/2207.12598)의 offical code와 논문을 참조하여 (Classifier-free, guidance) Speech Generation 및 Speech Enhancement PoC 수행

---


## File

</br>

### Speech to Text Model


<div align="center">
 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/E2E-STmodel.png width = "60%" height = "60%">


</div>




* CVSS_STT_multi-decoder.ipynb
    * Shared Encoder Multi Decoder STT 모델

* CVSS_STT_mutihead.ipynb
    * Shared Encoder Multi Decoder with muti-head attention  

</br>

### Speech Generation

<div align="center">
 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/diffusion_generation.png width = "60%" height = "60%">



</div>



https://github.com/user-attachments/assets/e5beef21-a87f-4b26-ba58-b739ed639c9a



https://github.com/user-attachments/assets/f67e02a4-eaa8-4a0c-b3f9-0aeb6d3d3e8a



https://github.com/user-attachments/assets/f5e264cb-ea51-43f1-b4aa-e465730439c1




* DDPM_Speech_free_Guided.ipynb
    * Audio MNIST Generation, DDPM (classifier-free)

* Speech_free_Guided_using_attention_with_DDIM_sampling.ipynb
    * Audio MNIST Generation, DDIM (classifier-free)

</br>


### Speech Enhancement

<div align="center"> 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/diffusion_enhance.png width = "60%" height = "60%">
</div>


https://github.com/user-attachments/assets/46a31d47-b026-418d-8700-0e0813e84035

**VTCK female(Ask her to bring these things with her from the store)**



https://github.com/user-attachments/assets/62cfb6d4-bc91-430f-b238-2ae1a43aa7e7

https://github.com/user-attachments/assets/338ed671-8d00-4272-a450-a61080784e38

https://github.com/user-attachments/assets/49ef35db-2a77-4542-9e2c-bea3aeb8b5be

https://github.com/user-attachments/assets/a0618afb-c92b-428c-96b8-e7676ced2976






* SDE_Speech_Enhancement.ipynb
    * Audio MNIST Speech Enhancement, SDE Diffusion Model  

* SDE_Speech_Guided.ipynb
    * Audio MNIST Speech Enhancement, SDE Diffusion Model (Classifier-Guided)

</br>







