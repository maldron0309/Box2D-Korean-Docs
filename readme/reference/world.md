---
description: 이 함수들은 시뮬레이션 월드를 생성할 수 있게 해줍니다.
---

# 월드(World)

### Data Structures

```c
struct b2RayResult
```

`b2World_RayCastClosest` 함수의 결과입니다.

```c
struct b2WorldDef
```

시뮬레이션 월드를 생성하는 데 사용되는 월드 구조체입니다.

```c
struct b2DebugDraw
```

Box2D 월드를 그리기 위해 구현할 수 있는 콜백을 보유하는 구조체입니다.



### Typedefs

{% code overflow="wrap" %}
```c
typedef void b2TaskCallback(int32_t startIndex, int32_t endIndex, uint32_t workerIndex, void *taskContext)
```
{% endcode %}

작업 인터페이스 이것은 Box2D 작업의 프로토타입입니다.

```c
// Some code
```
