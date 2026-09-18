# 🌐 Real-Time 3D Sorting Visualizer

> 웹 브라우저에서 실시간으로 정렬 알고리즘의 동작 과정을 탐색하고 학습할 수 있는 인터랙티브 3D 시각화 도구입니다.

[![GitHub Pages](https://img.shields.io/badge/Demo-GitHub%20Pages-4f8cff?style=flat-square&logo=github)](https://woodongho.github.io/SortingVisualizer/)
[![Three.js](https://img.shields.io/badge/WebGL-Three.js-black?style=flat-square&logo=three.js)](https://threejs.org/)
[![JavaScript](https://img.shields.io/badge/Language-Vanilla%20JavaScript-f7df1e?style=flat-square&logo=javascript)](https://developer.mozilla.org/ko/docs/Web/JavaScript)

🔗 **데모 바로가기**: [https://woodongho.github.io/SortingVisualizer/](https://woodongho.github.io/SortingVisualizer/)

---

## 📌 프로젝트 소개

**Real-Time 3D Sorting Visualizer**는 컴퓨터 과학의 핵심 기초인 정렬(Sorting) 알고리즘을 3차원 공간에서 시각화하여 원리를 직관적으로 이해할 수 있도록 설계된 교육용 웹 애플리케이션입니다.

평면적인 차트를 넘어 Three.js 기반의 입체 3D 큐브 블록과 조명, 실시간 회전 인터랙션, 의사코드 추적, 오디오 피치 효과를 통해 오감으로 알고리즘을 체득할 수 있습니다.

---

## ✨ 주요 기능

### 1. 🧊 몰입형 WebGL 3D 시각화
* **3D 입체 큐브 기둥**: 가로, 세로, 높이 및 실시간 조명 그림자가 적용된 3D 지오메트리 블록.
* **360° 자유 회전 & 줌**: 마우스 드래그 또는 모바일 터치 드래그로 씬 전체를 자유롭게 회전하고 핀치/휠로 확대/축소 가능.
* **시점 프리셋**: `3D 뷰`, `정면 뷰`, `탑뷰`, `시점 리셋` 버튼을 통해 원하는 앵글로 원클릭 전환.
* **상태별 3D 인터랙션**: 비교(Compare) 및 교환(Swap) 시 블록이 위로 붕 떠오르며 네온 발광 효과 제공.

### 2. 📚 교육용 알고리즘 가이드 & 실시간 분석
* **직관적인 실생활 비유 (Metaphor)**: 탄산 기포(버블), 카드 끼우기(삽입), 최강자 대진표(힙) 등 비전공자도 이해하기 쉬운 비유 제공.
* **단계별 작동 원리 & 장단점**: 각 알고리즘의 핵심 메커니즘과 실무 활용 팁 정리.
* **실시간 의사코드(Pseudocode) 추적**: 정렬 실행 중 현재 실행되고 있는 코드 라인을 실시간으로 하이라이트.
* **복잡도 분석표**: 최선(Best), 평균(Average), 최악(Worst) 시간 복잡도, 공간 복잡도 및 안정 정렬(Stable/Unstable) 뱃지 제공.

### 3. 🕹️ 세밀한 인터랙션 & 오감 피드백
* **한 단계씩 실행 (`한 단계 ▶|`)**: 디버깅하듯 1스텝(비교/교환)씩 실행하며 코드와 동작을 세밀하게 관찰 가능.
* **초기 배열 패턴 프리셋**:
  * 🎲 **무작위 (Random)**: 일반적인 무작위 데이터
  * 📈 **거의 정렬됨 (Nearly Sorted)**: 삽입 정렬의 $O(n)$ 성능 우수성을 확인
  * 📉 **역순 정렬 (Reversed)**: 최악의 케이스(Worst Case) 분석
  * 🔀 **중복 다수 (Few Unique)**: 동일한 키 값이 많을 때의 정렬 특성 관찰
* **Web Audio 피치 사운드**: 원소 값의 크기에 비례하는 주파수 사운드를 실시간 합성하여 청각적 피드백 제공 (음소거 지원).

### 4. 📱 모바일 & 태블릿 반응형 지원
* 화면 종횡비에 따른 카메라 거리 자동 보정으로 모바일 세로 모드에서도 잘림 없는 3D 뷰 제공.
* 터치 친화적 컴팩트 그리드 UI 레이아웃.

---

## 📊 지원 알고리즘 및 복잡도

| 알고리즘 | 최선 시간 | 평균 시간 | 최악 시간 | 공간 복잡도 | 안정성 (Stability) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Bubble Sort** (거품 정렬) | $O(n)$ | $O(n^2)$ | $O(n^2)$ | $O(1)$ | Stable (안정) |
| **Insertion Sort** (삽입 정렬) | $O(n)$ | $O(n^2)$ | $O(n^2)$ | $O(1)$ | Stable (안정) |
| **Selection Sort** (선택 정렬) | $O(n^2)$ | $O(n^2)$ | $O(n^2)$ | $O(1)$ | Unstable (불안정) |
| **Merge Sort** (병합 정렬) | $O(n \log n)$ | $O(n \log n)$ | $O(n \log n)$ | $O(n)$ | Stable (안정) |
| **Quick Sort** (퀵 정렬) | $O(n \log n)$ | $O(n \log n)$ | $O(n^2)$ | $O(\log n)$ | Unstable (불안정) |
| **Heap Sort** (힙 정렬) | $O(n \log n)$ | $O(n \log n)$ | $O(n \log n)$ | $O(1)$ | Unstable (불안정) |

---

## 🛠️ 기술 스택

* **Frontend**: HTML5, CSS3, Modern JavaScript (ES6+ Generator, Async/Await)
* **3D Graphics Engine**: [Three.js (r128)](https://threejs.org/) + `OrbitControls`
* **Audio**: Web Audio API (Synthesizer Oscillator)
* **Deployment**: GitHub Pages

---

## 🚀 로컬 실행 방법

별도의 빌드 도구나 의존성 설치 없이 웹 브라우저에서 바로 실행할 수 있습니다.

```bash
# 저장소 클론
git clone https://github.com/woodongho/SortingVisualizer.git

# 폴더 이동
cd SortingVisualizer

# 브라우저에서 바로 열기 또는 로컬 정적 서버 실행
python3 -m http.server 8080
```
브라우저에서 `http://localhost:8080`으로 접속합니다.

---

## 👤 Author

* **우동호 (woodongho)**
  * GitHub: [@woodongho](https://github.com/woodongho)
