# 시각장애인을 위한 도로 안내 로봇
> 기존에는 시각장애인이 안내견을 통해 길을 안내 받았다면 로봇을 통해 길을 안내 받을 수 있다고 생각.

[![NPM Version][npm-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Downloads Stats][npm-downloads]][npm-url]

- 이 프로젝트는 Jetbot이 트랙의 특정 경로를 따라가는 동시에 장애물을 인지하여 피함으로써 장애물에 부딪히는 일이 없도록 하는 것에 중점을 둠.
- 현재 안내견은 보통 시각장애인의 왼편에 서기 때문에 Jetbot의 경우에도 시각장애인의 왼편에 있다고 생각하고 장애물을 마주칠 경우 항상 오른쪽으로 피하도록 함
![image](https://user-images.githubusercontent.com/101259003/206101005-f7a882f5-4f69-40af-9c2d-c42257e1c5a8.png)


```[![이미지 텍스트](스크린샷 이미지)](유투브링크)```


gif로 움짤 올리기

```[![이미지 텍스트](gif 이미지)]```

<img src="https://user-images.githubusercontent.com/4470398/204947699-4feb33cd-ab75-41f6-bedd-10b22eb2e961.gif" width="400" height="280"/>



깃헙의 LFS를 설명해 놓은 동영상을 링크 

``` [![Video Label](http://img.youtube.com/vi/uLR1RNqJ1Mw/0.jpg)](https://youtu.be/uLR1RNqJ1Mw?t=0s) ```
[![Video Label](http://img.youtube.com/vi/E2rpPNNWpo4/0.jpg)](https://youtu.be/E2rpPNNWpo4) 



![](../header.png)

## 설치 방법

OS X & 리눅스:

```sh
npm install my-crazy-module --save
```

윈도우:

```sh
edit autoexec.bat
```

## 사용 예제

스크린 샷과 코드 예제를 통해 사용 방법을 자세히 설명합니다.

_더 많은 예제와 사용법은 [Wiki][wiki]를 참고하세요._

## 개발 환경 설정

모든 개발 의존성 설치 방법과 자동 테스트 슈트 실행 방법을 운영체제 별로 작성합니다.

```sh
make install
npm test
```

## 코드블럭 설명

```c
//```뒤에 자신이 원하는 언어 (생략 가능)
#include <stdio.h>
int main(void) {
  printf("Hello World!");
}
```


## 업데이트 내역

* 0.2.1
    * 수정: 문서 업데이트 (모듈 코드 동일)
* 0.2.0
    * 수정: `setDefaultXYZ()` 메서드 제거
    * 추가: `init()` 메서드 추가
* 0.1.1
    * 버그 수정: `baz()` 메서드 호출 시 부팅되지 않는 현상 (@컨트리뷰터 감사합니다!)
* 0.1.0
    * 첫 출시
    * 수정: `foo()` 메서드 네이밍을 `bar()`로 수정
* 0.0.1
    * 작업 진행 중

## 정보

이름 – [@트위터 주소](https://twitter.com/dbader_org) – 이메일주소@example.com

XYZ 라이센스를 준수하며 ``LICENSE``에서 자세한 정보를 확인할 수 있습니다.

[https://github.com/yourname/github-link](https://github.com/dbader/)

## README 

1. https://github.com/kyechan99/capsule-render
2. https://yermi.tistory.com/entry/%EA%BF%80%ED%8C%81-Github-Readme-%EC%98%88%EC%81%98%EA%B2%8C-%EA%BE%B8%EB%AF%B8%EA%B8%B0-Readme-Header-Badge-Widget-%EB%93%B1


## 그외의 팁

취소선
~~취소선~~


인용글
> 인용글 1
> > 인용글 2
> > > 인용글 3

기울임
*기울임 꼴*

_기울임 꼴_


굵은글씨

**굵은 글씨**

__굵은 글씨__

<!-- Markdown link & img dfn's -->
[npm-image]: https://img.shields.io/npm/v/datadog-metrics.svg?style=flat-square
[npm-url]: https://npmjs.org/package/datadog-metrics
[npm-downloads]: https://img.shields.io/npm/dm/datadog-metrics.svg?style=flat-square
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[wiki]: https://github.com/yourname/yourproject/wiki
