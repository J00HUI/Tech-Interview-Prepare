## Sorting
> 여러 곳 면접을 보면서 받았던 질문들
</br>

### 목차
1. Sorting Algorithm 에 Stable 하다는 것은 무엇을 의미하나요?
2. Sorting Algorithm 이 가짓수가 많은데 그 이유가 무엇일 것 같나요?
3. Quick sort 에 대해서 설명해줄 수 있나요?
</br>

---
### Q1. Sorting Algorithm 에 Stable 하다는 것은 무엇을 의미하나요?
동일한 Element 가 있을 때 정렬 전의 순서와 정렬 후의 순서가 동일함을 보장하는 것이 Stable 입니다.    
예를 들어 `[{k: 4, v:1}, {k: 3, v:2}, {k: 3, v:1}, {k: 2, v: 1}, {k: 5, v: 1}]` 을 stable 한 sorting algorithm 을 이용한다면,

`[{k: 2, v: 1}, {k: 3, v:2}, {k: 3, v:1}, {k: 4, v:1}, {k: 5, v: 1}]` 가 됩니다.   
(k 가 3인 Element 가 2가 있지만 input 된 순서 그대로 정렬됩니다.)   
</br>

### Q2. Sorting Algorithm 이 가짓수가 많은데 그 이유가 무엇일 것 같나요?
![image](https://user-images.githubusercontent.com/83942393/219272023-11ac42a0-d3be-4df4-9c30-04c43fbc894f.png)
</br>
(출처 : http://bigocheatsheet.com/)   

1. sorting algorithm 마다 expected 되는 속도가 다릅니다.
2. 속도가 아닌 Space Complexity 가 고려대상이 될 수 있습니다. Merge sort 같은 경우 insertion sort 나 selection sort 에 비해 추가 메모리 공간을 사용합니다.
3. Stable 한지 안한지에 따라 사용되어야 할 sorting algorithm 이 다를 수 있습니다.
</br>

### Q3. Quick sort 에 대해 설명해 줄 수 있나요?
Quick sort 는 Divide-and-Conquer paradigm 을 이용해 정렬을 수행하는 정렬 알고리즘입니다.   
그 중에서도 partitioning 이라는 아이디어를 사용합니다.   
partitioning 이란 pivot element 를 기준으로 왼쪽은 pivot 보다 작거나 같은 것을 모으고, 오른쪽은 pivot 보다 크거나 같은 것을 모아주는 것을 말합니다.   
partitioning 을 재귀적으로 진행하다보면 정렬이 완료됩니다.
</br>
</br>

---
#### Reference
https://github.com/qkraudghgh/coding-interview/blob/master/Interview/question/previous_interview.md#sorting-solution

