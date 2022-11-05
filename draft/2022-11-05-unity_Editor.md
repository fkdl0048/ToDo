---
title: "[Unity] Editor"
excerpt: " "

categories:
  - Unity
tags:
  - [Unity, Dev]

toc: true
toc_sticky: true
 
date: 2022-11-05
last_modified_at: 2022-11-05
---

# Custom Editor  

유니티에서 Editor를 사용자에 맞게 생성하거나 편집하는 방법은 크게 두가지로 나뉘는 것 같다.  

wizard editor를 이용하거나 editor를 커스텀 에디터를 만들거나..  

그 전에 Editor라고 한다면 개발 과정에서만 사용되는 `툴`이기 때문에 레벨을 잘 생각해야 한다.

따라서 빌드시에는 제외해야 하기 때문에 Editor이라는 폴더에 넣어서 스크립트를 관리한다.  

## [ExecuteInEditMode]  

[ExecuteInEditMode] 애트리뷰트는 play가 아니더라도 유니티 이벤트를 받아서 실행한다. 즉, 에디터레벨에서도 스크립트가 동작하게 할 수 있다.  



--- 

https://docs.unity3d.com/kr/2020.3/Manual/editor-CustomEditors.html
