# Developer_Setting
(Mac 기준) 개발 환경 세팅 가이드



## 1. 패키지 관리 brew 설치

​	brew.sh 접속 후 터미널에 입력

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```



설치 완료 후 터미널에 echo~, eval~ 두 줄 입력

![image-20220327221635726](/Users/dg/Library/Application Support/typora-user-images/image-20220327221635726.png)

터미널 종료 후 brew 커맨드로 잘나오는지 테스트



## 2. 필수 패키지 설치

```bash
brew install --cask firefox visual-studio-code google-chrome spotify brave-browser slack iterm2
```



#### 참조 터미널, iterm 세팅

1. Item -> preference -> appearance 접속 후 theme를 minimum으로 변경
2. Profiles -> sessions 드래그앤드롭으로  battery cpu memory 등 보고싶은 것 선택
3. Item color github dark로 세팅

#### Oh My Zsh 설치

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```



