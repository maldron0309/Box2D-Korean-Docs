---
description: 사용자 할당 함수의 프로토타입입니다.
---

# b2AllocFcn

```c
typedef void * b2AllocFcn(unsigned int size, int alignment)
```

**매개변수**:

* **size**: 할당할 크기(바이트 단위)
* **alignment**: 필요한 정렬 값으로, 2의 제곱수임이 보장됨
