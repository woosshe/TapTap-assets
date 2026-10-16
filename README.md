# TapTap assets

TapTap(안드로이드/아이폰 책 뷰어)이 필요할 때 골라 받는 파일 모음입니다.
항목마다 릴리스가 따로 있습니다(목소리 모델, 글꼴). 앱은 받은 파일마다 앱 안에 적힌 SHA-256 값과 맞는지 확인합니다.

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

## 글꼴 (릴리스 `fonts-v1`)

설정 › 글꼴에서 골라 받는 본문 글꼴입니다(앱에 들어 있는 숨바탕, 숨고딕은 빼고). 모두 SIL Open Font License 1.1 이고,
원본 파일을 고치지 않고 그대로 다시 올렸습니다. 글꼴마다 저작권 문구와 라이선스 전문을 같은 릴리스에 `OFL-이름.txt` 로 두었습니다.

- `Hahmlet-wght.ttf` 의 원래 이름은 `Hahmlet[wght].ttf` 입니다. 릴리스 파일 이름에 대괄호를 쓸 수 없어 이름만 바꿨고 내용은 같습니다.
- 글꼴만 따로 팔 수 없고, 고친 글꼴에는 원래 이름(예약된 글꼴 이름)을 쓸 수 없습니다. 자세한 조건은 각 라이선스 전문을 따릅니다.

| 글꼴 | 출처 | 라이선스 |
|---|---|---|
| 나눔명조 | google/fonts | OFL-nanummyeongjo.txt |
| 고운바탕 | google/fonts | OFL-gowunbatang.txt |
| 함렛 | google/fonts | OFL-hahmlet.txt |
| 송명 | google/fonts | OFL-songmyung.txt |
| 나눔고딕 | google/fonts | OFL-nanumgothic.txt |
| Pretendard | orioncactus/pretendard v1.3.9 | OFL-pretendard.txt |
| IBM Plex Sans KR | google/fonts | OFL-ibmplexsanskr.txt |
| 고딕 A1 | google/fonts | OFL-gothica1.txt |
| 나눔손글씨 펜 | google/fonts | OFL-nanumpenscript.txt |
| 나눔손글씨 붓 | google/fonts | OFL-nanumbrushscript.txt |
| 개구 | google/fonts | OFL-gaegu.txt |
| 연성 | google/fonts | OFL-yeonsung.txt |
| 푸어스토리 | google/fonts | OFL-poorstory.txt |
| 하이멜로디 | google/fonts | OFL-himelody.txt |
| 감자꽃 | google/fonts | OFL-gamjaflower.txt |
| Neo둥근모 Pro | neodgm/neodgm-pro v1.020 | OFL-neodgm-pro.txt |
| 갈무리11 | quiple/galmuri v2.40.4 | OFL-galmuri.txt |

google/fonts 는 커밋 5e8a3ba899557829a76cfdac30fa512bda91d7ca 의 파일입니다.

| 파일 | 글꼴 | SHA-256 |
|---|---|---|
| NanumMyeongjo-Regular.ttf | 나눔명조 | 7ed9e8653a8ed04285d51dc343ffea6eb3d9c73afc27383ea8929ee4ffd03205 |
| NanumMyeongjo-Bold.ttf | 나눔명조 | bc9ed8e60d93fe6db054b8fb988481b625f2eef8cb2317ad0e9834681b8fe3f3 |
| GowunBatang-Regular.ttf | 고운바탕 | 466c593e7147412e748af4856d5ad14709b5a860bdf62b9c2546f2c5874e9849 |
| GowunBatang-Bold.ttf | 고운바탕 | dbfcaa646e5831e7478524924f02906f550285a5050699b4e38c9950b3ec4b94 |
| Hahmlet-wght.ttf | 함렛 | 892bffe530255770a7435226154a02f519055ff6bedf64254f37f21d15a59279 |
| SongMyung-Regular.ttf | 송명 | 7f90ab20250911560212cc5819c7b205f9c6644bb96b65095d89fcae096bbf58 |
| NanumGothic-Regular.ttf | 나눔고딕 | 76f45ef4a6bcff344c837c95a7dcc26e017e38b5846d5ae0cdcb5b86be2e2d31 |
| NanumGothic-Bold.ttf | 나눔고딕 | f96298f9fb18e364d2370f4c3ce948ac67a2b61af992d7234bc15c42b033c674 |
| Pretendard-Regular.otf | Pretendard | 3ffbacde6ab8411f1d2db54bb9b1f0b3ee2a738932033722cf0388c06aed1c93 |
| Pretendard-Bold.otf | Pretendard | 2e91915fab54df71cc9598ebf608b2bdb54c6fe3c066ac61dff0bc44fca71cc7 |
| IBMPlexSansKR-Regular.ttf | IBM Plex Sans KR | 53750379270312368cf7641901f43a98dd892e3d9d5798cf25cdc245c85c71c0 |
| IBMPlexSansKR-Bold.ttf | IBM Plex Sans KR | 9d82a8be5330f6d7b53121262867b402baca672eb69b852928f06d185d357f7d |
| GothicA1-Regular.ttf | 고딕 A1 | 211151bea98098c579610ab1114bb1bfe909057207db561f357b896d076c21ac |
| GothicA1-Bold.ttf | 고딕 A1 | 2e883fa0ae548000996258b4101f2bb732a28b197264f49621a2cb16d6e9f126 |
| NanumPenScript-Regular.ttf | 나눔손글씨 펜 | 6f0d1ab29c7894010dc88831fb7a0a51edb79136e450344183de5b1a8b52bd43 |
| NanumBrushScript-Regular.ttf | 나눔손글씨 붓 | 27ceaf578c96f594cdf07fe0181b251790acbb746a164e45c1f6473f89911a31 |
| Gaegu-Regular.ttf | 개구 | aa52c98336f7c62e2896fc8b12b56a75d5b476d88a2f104b0980f4f7ce0adfc3 |
| Gaegu-Bold.ttf | 개구 | cc38a4af9506a45254d1ce07c589ec473d9e5f0be319e5a77b17c214903f8c1c |
| YeonSung-Regular.ttf | 연성 | 49ac2a11009f5f58307d377911eb45d210cf4c1d379d9eca38fb4cdad5491ef6 |
| PoorStory-Regular.ttf | 푸어스토리 | 831ab87f7b5463f9cd83ac249bf386816f3a478f1d226427c88cac907adb7ee2 |
| HiMelody-Regular.ttf | 하이멜로디 | 360d2c0a880918aa48328d1d9219f5390788d09a1c9353e12b471de018673ae6 |
| GamjaFlower-Regular.ttf | 감자꽃 | ece32819ed58536355a49a095b0cdfdd3b8ef9081c5ed9ca1cef8f5d999ae1ac |
| NeoDunggeunmoPro-Regular.ttf | Neo둥근모 Pro | e4b974b1a378ef1962e3c72dfbcb7b7bba09f54dd53bf57889af300b2531b155 |
| Galmuri11.ttf | 갈무리11 | 2c709890595668f7bdb6df408420fda957dde0288e95b31a1cc17a2ab98b4b4f |
| Galmuri11-Bold.ttf | 갈무리11 | 5265b2f437fe81f0c8095b44c0173dd9a276b58a42552bf983f21c0e69e6e8af |
