# GPT2-Assignment
GPT-2 기반 텍스트 생성 모델 구현 (Text Generation with GPT-2)
1. 프로젝트 개요
본 프로젝트는 Hugging Face의 'transformers' 라이브러리를 활용하여 OpenAI의 GPT-2(Generative Pre-trained Transformer 2) 언어 모델을 구현하고, 특정 프롬프트를 입력했을 때 문맥에 맞는 자연스러운 텍스트를 생성하는 모델을 구축하였습니다. 

본 모델은 Transformer 디코더(Decoder) 구조를 기반으로 하며, 방대한 양의 텍스트 데이터를 통해 사전 학습(Pre-training)된 언어 모델의 추론 성능을 검증하는 데 목적이 있습니다.
2. 개발 환경 및 라이브러리
Python: 3.10 이상
주요 라이브러리:
    'transformers': 사전 학습된 언어 모델 불러오기 및 텍스트 생성 파이프라인 구성
    'torch' (PyTorch): 딥러닝 연산 및 모델 실행 환경 제공
환경 설정:
'''bash
pip install transformers torch
3. 구현 상세
A. 모델 구조
모델: GPT-2 Small
Pipeline: text-generation 파이프라인을 활용하여 모델 로드부터 추론까지의 과정을 추상화
Tokenization: 입력된 텍스트를 모델이 이해할 수 있는 BPE(Byte Pair Encoding) 토큰으로 변환
B. 실행 방법
python main.py
4. 실행 결과 예시
Input Prompt: "Artificial Intelligence is"
Generated Output:
"Artificial Intelligence is not an abstraction from the physical world, but a means to an end. It is an extension of the human mind, and has become the standard for human behavior. The fact that it has been observed is a proof that our own consciousness is not a biological construct. It is a universal concept, a world of experience, and a source of inspiration."
