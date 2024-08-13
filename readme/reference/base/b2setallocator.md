---
description: 사용자가 메모리 할당 함수를 재정의할 수 있도록 합니다.  이 함수들은 애플리케이션 시작 시 설정되어야 합니다.
---

# b2SetAllocator()

<pre class="language-c"><code class="lang-c">
void b2SetAllocator(b2AllocFcn * allocFcn, 
<strong>                    b2FreeFcn * freeFcn )
</strong>
</code></pre>
