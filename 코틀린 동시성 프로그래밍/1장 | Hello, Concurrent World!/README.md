# 1장 | Hello, Concurrent World!
1장에서는 동시성이 무엇인지, 코틀린이 동시성 문제를 어떻게 다루는지 소개한다.

### 💡 이 장에서 다루는 주제
- 프로세스, 스레드, 코루틴 및 이들의 관계
- 동시성 소개
- 동시성 대 병렬성
- CPU 바운드 및 I/O 바운드 알고리즘(CPU 집중 및 I/O 집중 알고리즘)
- 동시성이 망설여지는 이유
- 코틀린의 동시성
- 개념과 용어

### 📝 목차
- 프로세스, 스레드, 코루틴
  - [프로세스](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/프로세스%2C%20스레드%2C%20코루틴.md#1-프로세스)
  - [스레드](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/프로세스%2C%20스레드%2C%20코루틴.md#2-스레드)
  - [코루틴](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/프로세스%2C%20스레드%2C%20코루틴.md#3-코루틴)
  - [내용 정리](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/프로세스%2C%20스레드%2C%20코루틴.md#white_check_mark-내용-정리)
  - [동시성에 대해](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/동시성.md#1-동시성에-대해)
  - [동시성은 병렬성이 아니다](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/동시성.md#2-동시성은-병렬성이-아니다)
  - [CPU 바운드와 I/O 바운드](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/CPU%20바운드와%20IO%20바운드.md#1-cpu-바운드와-io-바운드)
  - [CPU 바운드 알고리즘에서의 동시성과 병렬성](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/CPU%20바운드와%20IO%20바운드.md#2-cpu-바운드-알고리즘에서의-동시성과-병렬성)
  - [I/O 바운드 알고리즘에서의 동시성 대 병렬성](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/CPU%20바운드와%20IO%20바운드.md#3-io-바운드-알고리즘에서의-동시성과-병렬성)
  - [동시성이 어려운 이유](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/동시성이%20어려운%20이유.md)
- 코틀린에서의 동시성
  - [넌 블로킹](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/코틀린에서의%20동시성.md#no_entry_sign-넌-블로킹)
  - [명시적인 선언](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/코틀린에서의%20동시성.md#bangbang-명시적인-선언)
  - [코틀린 동시성 관련 개념과 용어](https://github.com/jionchu/Read-Dev-Book/tree/main/코틀린%20동시성%20프로그래밍/1장%20%7C%20Hello%2C%20Concurrent%20World!/코틀린에서의%20동시성.md#ab-코틀린-동시성-관련-개념과-용어)