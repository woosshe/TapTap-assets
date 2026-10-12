# TapTap assets

TapTap(안드로이드/아이폰 책 뷰어)이 필요할 때 골라 받는 파일 모음입니다.
항목마다 릴리스가 따로 있습니다. 앱은 받은 파일마다 앱 안에 적힌 SHA-256 값과 맞는지 확인합니다.

## supertonic-2 (릴리스 `supertonic-2-v1`)

소설 듣기에 쓰는 목소리 모델입니다. 한국어, 영어, 스페인어, 포르투갈어, 프랑스어를 읽고 화자 10명이 들어 있습니다.

| 파일 | SHA-256 |
|---|---|
| duration_predictor.int8.onnx | 6d556b3691165c364be91dc0bd894656b5949f5acd2750d8ec2f954010845011 |
| text_encoder.int8.onnx | dd5f535ed629f7df86071043e15f541ce1b2ab7f1bdbce4c7892b307bca79fa3 |
| vector_estimator.int8.onnx | 9cce89801068dc998719fbc91777f99f3f4d16ee36592281f8703f32e305daa2 |
| vocoder.int8.onnx | db99c36fb871fbfb128b903662995f2e22213e875f2434f319f8d10ee0f10e90 |
| tts.json | ee531d9af9b80438a2ed703e22155ee6c83b12595ab22fd3bb6de94c7502fe96 |
| unicode_indexer.bin | 06557ec23778a2c67130a99e28f5f550b9598fc1f04049cbb35d864549913154 |
| voice.bin | 12e0919ffc641ff20858026a4c655fbd9e5c414800bb1b756c9d4011e2536325 |

- 모델: Supertone Inc. 의 [Supertonic 2](https://huggingface.co/Supertone/supertonic-2)
- 변경 사항: 원본을 sherpa-onnx 프로젝트가 int8 로 줄여 ONNX 로 내보낸 파일입니다
  ([tts-models](https://github.com/k2-fsa/sherpa-onnx/releases/tag/tts-models) 릴리스의 `sherpa-onnx-supertonic-tts-int8-2026-03-06`).
  여기에는 그 파일을 고치지 않고 낱개로 다시 올렸습니다.
- 라이선스: BigScience Open RAIL-M, 전문은 [MODEL-LICENSE](MODEL-LICENSE)에 있습니다.
  **이 모델은 그 라이선스 5항과 부록 A의 사용 제한을 따라야 합니다.**
  (예: 남을 사칭하거나 속이는 데, 법을 어기는 데 쓰면 안 됩니다)
