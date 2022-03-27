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

powerlevel10k github

Installation -> oh my zsh

git clone 커맨드 복사 후 터미널에서 실행

```bash
code ~/.zshrc
```

ZSH_THEME = "robberssell" -> "powerlevel10k/powerlevel10k"

어플리케이션 재시작 후 환경설정에서 취향에 따라 선택



## 개발환경 세팅

```bash
brew install python3 go pipenv nvm gh
```

![image-20220328001223270](/Users/dg/Library/Application Support/typora-user-images/image-20220328001223270.png)

해당 커맨드 복사 후 code에서 실행 후 제일 마지막 줄에 붙여넣기 저장

```bash
code ~/.zshrc
```



터미널 재시작 후 nvm 설치 확인

```bash
nvm	ls-remote
```

```bash
nvm install 17.3.1
nvm install 16.13.2
# 둘 다 설치 후 버젼관리
nvm use default # 17.3.1 사용
nvm use 16.13.2 # 16.13.2 사용
```

