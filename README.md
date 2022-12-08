## 왜 Rust를 배워야 하는가?
- 2021년 4분기 기준 Github 점유율 15위 언어
- C++ 암살자 포지션 (개인적으로 10년안에 C++ 넘어설 듯)
- 블록체인, 임베디드, 시스템프로그래밍, 서버, 분산처리, WASM 등에서 활발히 사용되는 고성능 언어
- 모던하고 깔끔한 언어 디자인, 훌륭한 개발툴과 패키지 매니저
- 수준높은 사용자들과 커뮤니티, 독보적인 UX를 기반으로 한 철옹성 같은 팬덤들

## Rust the 'insightful language'
- Rust는 기본적으로 '멀티패러다임' 언어
- Rust는 사용법이 복잡하고 언어 디자인에 녹아있는 컴퓨터공학적, 프로그래밍언어론적인 배경이 깊음
- 다른 말로, Rust를 잘 배우면 Rust를 잘 하는 사람이 되는게 아니라 제너럴하게 프로그래밍을 잘 하는 사람이 됨
- 따라서 Rust만 잘 배우면 다른 언어 (특히 Python, JS 같은 언어)는 길어도 3주안에 현업에서 사용할 정도로 트랜지션이 가능함
- Rust의 로우레벨적 내용(FFI, Async, 컴파일러 내부 등)까지 익히게 된다면 컴퓨터공학 전반에 걸쳐 이론적인 이해도가 상당할 것으로 예상
- 따라서 Rust를 배우는 것은 매우 인사이트풀하며 수준높은 학습임

## Rust in Blockchain
- 블록체인에서 Solidty, Go와 함께 사용자가 제일 많은 3강 언어
- Solidity는 컨트랙트에서만 쓰이고, Go는 노드구현에서만 쓰이지만 Rust는 컨트랙트와 노드구현 전부쓰임(!)
- Parity Ethereum, LightHouse, Substrate(Polkadot), Solana, Near Protocol, zkSync,
CosmWasm(Cosmos), Tendermint&IBC(informal), Sui, eWASM, Foundry, Aptos 등이 Rust로 만들어진 유명 프로젝트

## 설치해야하는 것들
- git
- vscode
- vscode extension: Rust Analyzer (얘 말고 다른거 깔지마세요)

## 자료

### The Rust Programming Language
https://docs.rs/
일명 'TRPL'. [링크](https://doc.rust-lang.org/book/)
- Rust를 공부하는 큰 플로우를 제시해주는 제일 중요한 자료
- TRPL을 정독하는 것이 Rust 공부의 메인 컨텐츠
- 정말 필요한 내용을 서사적으로 잘 전개하면서 서술 해놨으니 그냥 고시공부 하듯이 딱 앉아서 읽으면 됨

### Crate std
Rust의 스탠다드 라이브러리 (std)에 대한 레퍼런스. [링크](https://doc.rust-lang.org/std/)
- Rust는 스탠다드 라이브러리가 (다른 언어에 비해) 깔끔하고 강력하며 완결성있다. 따라서 자주 쓰게 될 것
- 스탠다드 라이브러리 요소들을 쓰다가 잘 모르겠으면 여길 보면 된다.

### easy_rust
Rust를 '쉬운 영어'로 간결하게 설명한 자료. [링크](https://github.com/Dhghomon/easy_rust)
- TRPL보다 더 간략하고 핵심만 담백하게 뽑아놨음
- Rust를 속성으로 배워야한다면 TRPL보다 이걸 정독하는게 나음
- Rust를 정석으로 배우고 싶다면 일단 메인 자료는 TRPL로 삼고,
easy_rust는 그냥 머리 식히면서 다른 관점의 서술을 참고하거나, 전반적인 아웃라인을 따라가는 용도로 사용

### Rust by Example
Rust 코드의 예시들을 모아놓은 친절한 곳. [링크](https://doc.rust-lang.org/rust-by-example)

### Reference
Rust 언어의 Specification. [링크](https://doc.rust-lang.org/stable/reference/)
- Rust의 어떤 문법적 요소에 대한 포멀한 스펙을 가끔 보고 싶을때 참고하면 된다.

## 자주 쓰게 될 써드파티 라이브러리
- [serde](https://serde.rs/)
- [thiserror](https://docs.rs/thiserror)
- [futures](https://docs.rs/futures)
- [tokio](https://docs.rs/tokio)

## 앞으로 어떤 여정이?
만약 TRPL을 다 공부했다면 다음과 같은 심화판이 남아있다.
- [Rustonomicon](https://doc.rust-lang.org/nomicon/): Rust의 `unsafe`기능을 비롯한 온갖 딥한 내용을 설명하는 금서
- [Asynchronous Programming in Rust](https://rust-lang.github.io/async-book): Rust의 킬링피쳐중 하나인 비동기프로그래밍 사용법에 대한 가이드

## 기타 꿀팁
- 질문방에 코드 올리고 질문할 때에는 텍스트 그대로 복붙하지말고 [Rust Playground](https://play.rust-lang.org/)를 사용하자. 컴파일러 없는 환경에서 웹으로 간단히 Rust코딩을 해볼 수도 있고, 'Share'버튼 누르면 링크로 코드를 다른 사람한테 줄 수 있다.
