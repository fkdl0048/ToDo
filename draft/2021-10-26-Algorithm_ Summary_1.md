---
title:  "알고리즘[BaekJoon 9202]"
excerpt: " "

categories:
  - Algorithm
tags:
  - [Algorithm, Study]

toc: true
toc_sticky: true
 
date: 2021-10-26
last_modified_at: 2021-10-26

---

## 🔎 BaekJoon [Boggle 9202]  

<https://www.acmicpc.net/problem/9202>  

이 문제는 재귀함수, 완전탐색을 사용하여 전체 단어의 수를 찾는 문제이다..!  

c언어로 풀려고 하니 막히는 부분이 많지만..! 끝까지 풀어보는걸로,,!

```c
#include <stdio.h>
#include <stdlib.h>
#include <malloc.h>

int main(){
    int i,j;
    int wordNum,arrNum;
    char **str;
    char arr[5][5];

    scanf("%d",&wordNum);
    str = (char **)malloc(sizeof(char*) * wordNum);
    if(str == NULL)
        return 0;
    for (i = 0; i < wordNum; i++){
        str[i] = (char *)malloc(sizeof(char) * 9);
        if (str[i] == NULL)
            return 0;
        scanf("%s",str[i]);
    }
    
    scanf("");
    
    scanf("%d",&arrNum);

    while (arrNum)
    {
        for (i = 0; i < 4; i++){
            scanf("%s",arr[i]);
        }
        
        arrNum--;
        scanf("");
    }
    
    for (i = 0; i < wordNum; i++)
    {
        printf("%s ", str[i]);
        printf("%d\n",_msize(str[i]));
    }

    for (i = 0; i < 4; i++)
    {
        printf("%c\n",arr[i][0]);
    }

    return 0;
}
```

진행중 ㅠㅠ..