# 오픈소스소프트웨어

## Week1-1 강의 개요 [(강의계획서)](https://rptbi.jnu.ac.kr/ReportApp/stdhak/reportView.aspx)
* ### 교과요목
  1. 오픈소스 소프트웨어 개발을 위한 기본 개념과 도구 , 특히 소스 코드 버전 컨트롤과 패키지 관리, 프로젝트 빌드를 중점으로 배운다.
  2. 애자일 기반 소프트웨어 개발 방법인 짝 프로그래밍, 테스트 주도 개발, 행위 주도 개발, 클라우드 기반 데브옵스를 공부한다.
  3. 새로운/낯선 소프트웨어 개발 환경 및 도구를 스스로 배우는 태도를 배우는 것을 목적으로 한다.  

  **새로운 추세의 컴퓨팅 환경에 빠르게 적응하여 협력적인 소프트웨어 개발을 주도할 수 있는 능력을 배운다.**
* ### 대학 핵심 역량
  1. _컴퓨팅사고_  
  함수형 프로그래밍언어 스타일을 익힘
  2. _융합_  
  LLM/ChatGPT를 새로윤 프로그래밍을 배우는데 활용
  3. _글로컬_  
  Git/Github를 통해 협업하는 방식을 배움  
  영어 학습 자료를 공부함으로써 영어 활용 기회를 늘림
* ### 전공 능력  
    **소프트웨어 응용 문제해결 능력**
* ### 수업 방법  
    강의, 플립러닝, 실험실습
* ### 평가
  * 중간고사(30%)
  * 기말고사(40%)
  * 개별과제(20%)
  * 출석(10%)  
  동영상(5%)/퀴즈(5%)

## Week1-2 오픈소스소프트웨어 개요
* ### 오픈 소스 소프트웨어란?  
    : 소프트웨어 저작권 소유자가 _모든 사람에게_ 소스 코드를 게시, 사용, 복사, 수정 및 배포할 권리를 부여한 소프트웨어
* ### Free Software vs. Open Source Software
  * Free Software(**자유** 소프트웨어)
    * Richard Stallman - Creator of GNU Project  
    ![Richard Stallman](https://images.app.goo.gl/MJYQj4wmNaSA4M978)
    * FSF (Free Software Foundation, 1984~)  
    GPL 1.0(1989), GPL 2.0(1991), GPL 3.0(2007)
    * Copyleft (No SW patent, No DRM)
  * Open Source Software
    * Eric S. Raymond - Author of 'The Cathedral and thr Bazzar(성당과 시장)'  
    ![Eric S. Raymond](https://images.app.goo.gl/dtGRoBFXjTQS8gJi8)
    * OSI (Open Source Initiative, 1998~)
      * AMbiguity of 'free'
      * Combination of OSS and Closed Source SW
      * License under law
* ### OSS 라이선스    
    : 오픈 소스 소프트웨어의 사용, 복제, 수정, 배포 권한의 **범위**를 지정
  * GPL (GNU General Public License)
  * LGPL (GNU Lesser General Public License)
  * MIT License
  * BSD License
  * Apache License
  * MPL (Mozilla Public License)

## Week2-1 버전 관리 개요
* ### Version Control System (VCS)  
  : Track your files over time so that you can easily get back to a previous working version  

  VCS software
  * CVS (Concurrent Version System)
  * _SVN (Subversion)_
  * Mercurial
  * Darcs
  * _**Git**_

  Repository or Repo (저장소)

* ### General Actions in VCS
  * Checkin  
  : Check in a file and modify it over time
  * Checkout and editing  
  : Check out, edit, and check in a file
  * Diffs  
  : The trunk has a history of changes as a file evolves
  * Branching  
  : Copy code into a separate folder so we can have a separate history of changes
  * **Merging**  
  : Merge changes from one branch to another
  * Conflicts
  * **Tagging**  
  : Let you tag any revision for easy reference such as 'Release 1.0' instead of r4

* ### Two Main Types of VCS
  * Centralized VCS
    * One central repository with many users
    * E.g. CVS, _SVN_, Darcs
  * Decentralized(Distributed) VCS
    * Every iser owns his or her local repository
    * A separate remote(central) repository  
    : Sometimes, more than one remote(central) repositories
    * Two new actions (with remote repositories)  
    : fork, pull request
    * **Git**, Mercurial

## Week2-2 Git
* ### Linus Torvalds  
    : for collaboration of development of Linux kenel

* ### A distributed version control system
  * Workspace  
  : files you are working with
  * Index  
  : (staged) files to be considered in the next commit
  * Local repository  
  : files committed to the local repo
  * Remote repositoroy  
  : files pushed to the remote repo

## Week2-3 Github, fork, pull request
* ### GitHub  
    : Git-based Source Code Hosting for Social Coding
    * fork  
    : OSS repo의 remote repo를 나의 repo에 remote repo를 만드는 것
    * pull request  
    : 나의 repo의 원격 저장소의 내용을 다시 OSS repo의 원격 저장소로 보내는 것

## Week2-4 Git: Advanced topics

## Week3 Markdown
* ### _Italics_ and **Bold**  
  * 이탤릭체는 텍스트 앞뒤로 _을 붙임
  * 볼드체는 텍스트 앞뒤로 **을 붙임

* ### Headers
  * 구문 앞에 #을 붙임
  * 원하는 헤더 크기와 동일한 개수 #로 생성
  * 총 6개의 크기로 구분

* ### Links
  * 인라인 링크  
  : [텍스트](링크 주소)
  * 참조 링크  
  : [텍스트][태그], 마크다운 페이지 맨 밑에 [태그]: 링크 주소
    * 다중 링크 시 링크를 변경할 때 한 번의 변경만으로 모두 변경 가능

* ### Images
  * 인라인 이미지  
  : ![대체 텍스트](이미지 링크 주소)
  * 참조 이미지  
  : ![대체 텍스트][태그], 마크다운 페이지 맨 밑에 [태그]: 이미지 링크 주소

* ### Blockquotes
  * 문장 앞에 >붙여 생성
  * 인용문이 여러 단락인 경우 공백 라인 포함 모든 라인에 >붙여 하나의 인용문으로 생성 가능

* ### LIst
  * 순서 없는 것 (unordered)  
  : 각 항목 앞에 *을 붙임, 각 항목은 하나의 라인
  * 순서 있는 것 (ordered)  
  : *대신 숫자를 붙임
  * 앞의 항목보다 공백 한 칸을 *앞에 더 들여써 하위 리스트 생성

* ### Paragraphs
  * 한 단락 내 줄 바꿈은 각 줄의 끝에 2번의 공백을 넣어 가능
  * 단락 구분은 공백 한 줄로