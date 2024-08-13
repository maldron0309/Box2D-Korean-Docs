# 기본(Base)

기본 기능 더 보기...

### Data Structures

```c
struct b2Version
 	버전 번호 체계 (Version numbering scheme). 더 보기...
```

### Typedefs

```c
typedef void * 	b2AllocFcn(unsigned int size, int alignment)
                사용자 할당 함수(user allocation function)의 프로토타입.
```

```c
typedef void 	b2FreeFcn(void *mem)
                사용자 해제 함수(user free function)의 프로토타입.
```

```c
typedef int b2AssertFcn(const char *condition, const char *fileName, int lineNumber)
사용자 어설트 콜백(user assert callback)의 프로토타입. 디버거 중단을 건너뛰려면 0을 반환합니다.
```

### Functions

```c
void b2SetAllocator (b2AllocFcn *allocFcn, b2FreeFcn *freeFcn)
     이것은 사용자가 할당 함수(allocation functions)를 재정의할 수 있게 합니다.
```

```c
int b2GetByteCount (void)
```

```c
void b2SetAssertFcn (b2AssertFcn *assertFcn)
     기본 어설트 콜백(assert callback)을 재정의합니다.
```

```c
b2Version b2GetVersion (void)
          Box2D의 현재 버전을 가져옵니다.
```

### Detailed Description

기본 기능

### Data Structure Documentation

{% tabs %}
{% tab title=" b2Version" %}
```c
struct b2Version
```

버전 번호 체계.

&#x20;[https://semver.org/](https://semver.org/) 참조

<table><thead><tr><th>Data Fields</th><th></th><th></th><th data-hidden></th><th data-hidden></th></tr></thead><tbody><tr><td>int</td><td>major</td><td>중요한 변경사항</td><td></td><td></td></tr><tr><td>int</td><td>minor</td><td>점진적 변경사항</td><td></td><td></td></tr><tr><td>int</td><td>revision</td><td>버그 수정</td><td></td><td></td></tr></tbody></table>

\

{% endtab %}
{% endtabs %}

### Typedef Documentation

{% tabs %}
{% tab title="b2AllocFcn" %}
```c
typedef void * b2AllocFcn(unsigned int size, int alignment)
```

사용자 할당 함수(user allocation function)의 프로토타입.

매개변수

* size : 할당 크기(바이트 단위)
* alignment : 필요한 정렬(alignment), 2의 거듭제곱으로 보장됨

\

{% endtab %}
{% endtabs %}
