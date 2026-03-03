# Week1 - Today's Crypto Prices (CoinGecko)

Data source (CoinGecko API):
`https://api.coingecko.com/api/v3/simple/price?ids=bitcoin,ethereum&vs_currencies=usd,krw`

## Today's Prices

| Coin | USD | KRW |
|---|---:|---:|
| Bitcoin (BTC) | 여기에_USD | 여기에_KRW |
| Ethereum (ETH) | 여기에_USD | 여기에_KRW |

## What I did (Step-by-step)

1. `blockchain_training`이라는 GitHub 저장소를 생성하였다.
2. GitHub Pages를 활성화하여 웹페이지를 배포하였다.
3. `week1` 폴더를 생성하고, `index.html` 파일을 작성하였다.
4. HTML과 CSS를 사용하여 비트코인(Bitcoin)과 이더리움(Ethereum)의 가격을 표시하는 대시보드 형태의 표를 구현하였다.
5. JavaScript의 `fetch()` 함수를 사용하여 CoinGecko API에서
   비트코인과 이더리움의 USD 및 KRW 가격 데이터를 가져오도록 구성하였다.
6. 브라우저에서 CoinGecko API 호출 시 CORS 오류가 발생하였다.
7. CORS 문제를 해결하기 위해 CORS 프록시(`https://corsproxy.io/`)를 활용하여
   CoinGecko API에 접근하도록 수정하였다.
8. API 요청 시 캐시 및 429(Too Many Requests) 오류를 방지하기 위해
   요청 URL에 타임스탬프를 추가하였다.
9. `setInterval()` 함수를 사용하여 30초마다 자동으로 가격을 갱신하도록 구현하였다.

10. 가격이 갱신될 때 시각적으로 표시되도록 애니메이션 효과를 추가하였다.
