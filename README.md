# Speech to Speech Translation(S2ST) with Diffusion Model




<div align="center">
 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/S2ST_abs.png width = "80%" height = "80%">

**S2ST Model**

</div>


* 기존 S2ST 모델은 ASR-> MT->TTS로 이루어진 Cascaded S2ST 형태, 이는 학습 시에 많은 데이터와 시간 그리고 컴퓨팅 소소를 요구함.
* 해당 문제들을 완화하기 위해 본 연구에서는 E2E 방식의 S2ST 기술의 연구를 진행.
* 최근 Diffusion Model은 생성 AI 분야에서 두각을 드러냄. 기존 생성 AI 모델 GAN과 비교하여 명시적으로 확률적 모델링을 기반으로 학습하기에 Mode Collapse의 빈도가 적으며, MultiModal 데이터 기반의 생성에서 경쟁력이 있음.
* 본 연구에서는 Diffusion Model을 활용하여 입력 화자의 음성 특징을 보존한 채 target 언어로 변환된 음성 생성을 생성하는 S2ST 모델 설계를 시도. 

</br>





DDPM 및 [SDE Diffusion Model](https://colab.research.google.com/drive/120kYYBOVa1i0TD85RjlEkFjaWDxSFUx3?usp=sharing#scrollTo=8PPsLx4dGCGa)의 튜토리얼 코드를 기반으로 [Classifier-Guided Diffusion Model](https://github.com/openai/guided-diffusion/tree/main), [Classifier-free Diffusion Model](https://arxiv.org/abs/2207.12598)의 offical code와 논문을 참조하여 (Classifier-free, guidance) Speech Generation 및 Speech Enhancement PoC 수행

---


## File

</br>


<div align="center">
 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/E2E-STmodel.png width = "60%" height = "60%">

**Speech to Text Model**

</div>








* CVSS_STT_multi-decoder.ipynb
    * Shared Encoder Multi Decoder STT 모델

* CVSS_STT_mutihead.ipynb
    * Shared Encoder Multi Decoder with muti-head attention  

</br>



<div align="center">
 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/diffusion_generation.png width = "60%" height = "60%">

**Speech Generation**

</div>







* DDPM_Speech_free_Guided.ipynb
    * Audio MNIST Generation, DDPM (classifier-free)

* Speech_free_Guided_using_attention_with_DDIM_sampling.ipynb
    * Audio MNIST Generation, DDIM (classifier-free)

</br>



<div align="center">
 
<img src = https://github.com/kkkkkkkm/Diffusion/blob/main/img/diffusion_enhance.png width = "60%" height = "60%">

**Speech Enhancement**

</div>


<audio controls>
    <source src=./img/vctk_origin.wav>
</audio>

https://github.com/kkkkkkkm/Diffusion/blob/main/img/vctk_origin.wav

* SDE_Speech_Enhancement.ipynb
    * VCTK Speech Enhancement, SDE Diffusion Model  

* SDE_Speech_Guided.ipynb
    *  VCTK Speech Enhancement, SDE Diffusion Model (Classifier-Guided)

</br>

### 이건 내용
안녕하세요, [교수님 성함] 교수님.
저는 [현재 소속 학교 및 학과]에서 [전공 분야]를 공부하고 있는 [본인의 이름]입니다. 교수님의 연구 분야인 [교수님의 주요 연구 분야]에 깊은 관심을 가지고 박사 과정 지원과 관련하여 문의드리고자 이렇게 메일을 드립니다.

[교수님의 논문이나 연구를 구체적으로 언급하며 관심 표현] 예를 들어, "특히 교수님께서 [논문 제목이나 연구 주제]를 통해 [연구 주제나 성과]를 이루신 점에 깊은 감명을 받았으며, 해당 연구가 [본인의 연구나 관심사와 관련된 내용]과 맞닿아 있어 더욱 큰 관심을 갖게 되었습니다."

저는 [본인의 연구 경력, 전공, 학업 성과]를 통해 [해당 연구 주제와 관련된 경험 또는 관심]을 쌓아왔습니다. 예를 들어, 저는 [주요 연구 성과, 프로젝트 경험, 석사 논문 주제 등]를 통해 [자신의 역량]을 다져왔으며, 이를 바탕으로 교수님의 연구실에서 더욱 심도 있는 연구를 진행하고 싶습니다.

[입학 시기 및 연구 방향 언급]
만약 가능하다면, [입학 희망 시기]부터 교수님의 연구실에서 박사 과정을 시작하며 [구체적인 연구 주제 또는 관심 분야]에 대해 연구를 진행하고 싶습니다. 제가 교수님의 연구실에 합류하여 [연구실에 기여할 수 있는 점 또는 목표]에 대해 함께 논의할 기회를 주시면 감사하겠습니다.

교수님의 바쁘신 일정에도 불구하고 제 메일을 읽어주셔서 감사드립니다. 제 프로필이나 성과를 더 자세히 보고 싶으시면 첨부된 CV를 참고해 주시기 바랍니다. 혹시 더 필요한 자료나 정보를 요청해 주신다면 기쁜 마음으로 제공해 드리겠습니다.
감사합니다. 답신 기다리겠습니다.

좋은 하루 되시길 바랍니다.
감사합니다.




국립농업과학원의 유전자 공학과에서는 식물 표현체를 탐지하고 이를 기반으로 생산량을


국립농업과학원에서 식물의 표현체를 탐지하는 과제를 진행하던 와중 시계열과 같은 센서 데이터 

------------


https://brunch.co.kr/@j-wisdom/15

https://blog.naver.com/aidway/222129883667
ultralytics
나는 2024년에 컴퓨터공학 석사를 졸업하고 현재 국립농업과학원에서 석사후연구원을 수행하는 김강민이다. 

농과원에서 식물 표현체 탐지 과제를 수행하며, 산업 데이터를 활용한 인공지능에 관심이 생겼다.
>> 

나는 석사과정 동안 자연어 처리와 더불어 음성을 융합하는 연구를 진행하며 Transformer나 Diffusion Model 같은 딥러닝 활용 능력을 다져왔으며, 이를 바탕으로 산업계에 적용 가능한 기술을 위한 연구를 진행하고 싶다.

만약 가능하다면 2025년도 9월 부터 입학하여 박사 과정을 시작하고자 하며, 이를 위해 면담을 요청드리고 싶습니다.

교수님의 바쁘신 일정에도 불구하고 제 메일을 읽어주셔서 감사드립니다. 제 프로필이나 성과를 더 자세히 보고 싶으시면 첨부된 CV를 참고해 주시기 바랍니다.


----------------
상승효과를 이끌어내는
안녕하십니까, 저는 다양한 데이터와 딥러닝을 접목시켜 실용적인 AI 전문가로 거듭나고자 고려대학교대학원에 지원한 김강민 입니다.
저는 산업 현장의 활용하여 Anomaly Detection, Multivariate Time Series Modeling와 같은 연구를 수행하고 싶습니다.


[산업 데이터에 관심]
저는 국립농업과학원에서 식물의 표현체를 탐지와 이를 활용한 수확량 예측 과제를 지원하게 되었습니다. 이를 수행하며 깨달은 점은 Vision AI의 적용이 쉽지 않다는 것이었습니다. 자동으로 식물체 이미지 데이터를 수집하기 위한 고가의 기기가 존재하였지만, 과제의 수행을 위해서 라벨링이 수작업으로 진행되어야 했고, 관련 지식이 부족하다면----

Vision AI의 적용이 쉽지 않다는 것을 알았다. 이곳에는 데이터를 자동으로 수집하기 위한 고가의 기기가 존재했지만 모델을 학습시키기 위한 수작업 라벨링 인력은 부족했다. 라벨링을 수행되었더라도 적합한 지식의 부재와 사람들이 엄격한 라벨링 표준을 지키지 않아 결국 모델의 성능은 유의미한 결과를 낼 수 없었다. Vision을 위한 원시 데이터는 존재하지만 막상 쓸수는 없는 상황이었던 곳이었는데, 그럼에도 비료의 시비양, 스마트 온실의 환경 데이터, 식물의 형질 조사를 통해 기록된 수치 값과 같은 정형 데이터는 존재했다. 문득 별도로 돈과 시간을 넣어 Vision AI과 딥러닝을 위한 위한 값비싼 설비들을 도입하는 모든 기업과 산업에서도 멀티모달을 통해 센서 데이터를 사용할 것 이라는 생각이 들었고, 실용성을 바탕으로 세상의 변화에 기여할 수 있는 분야는 산 <<
이러한 능력을 바탕으로 기업에게는 효율적으로 비용을 절감할 수 있도록 해주는 동시에 소비자에게는 보다 나은 제품을 저렴하게 구입할 수 있는 기회를 제공해 주는 것입니다.

산업경영공학이 다른 공학분야와 뚜렷한 차이가 나는 점은 크게 두 가지를 들 수 있습니다. 그 하나는 다른 공학분야는 한정된 분야에만 적용 가능하지만, 산업경영공학은 매우 다양한 분야에서 활동할 기회를 제공해 주며, 이러한 한정된 각개의 개별 분야를 전체적인 입장에서 조율하고 관리하여 최적의 조건을 이끌어 낸다는 점입니다.






