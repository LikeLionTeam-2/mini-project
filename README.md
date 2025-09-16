# 🚀 멋쟁이사자처럼 회고 2조

## 📌 개요

팀원들이 협업하며 성장하고, 정기적인 회고를 통해 개선점을 찾아갑니다.

## 👥 팀원

<table>
    <tr>
        <td align="center"><a href="https://github.com/Hae-in"><img src="https://avatars.githubusercontent.com/Hae-in" width="130px;" height="130px" alt=""></a></td>
        <td align="center"><a href="https://github.com/seongsiyoung"><img src="https://avatars.githubusercontent.com/seongsiyoung" width="130px;" height="130px" alt=""></a></td>
        <td align="center"><a href="https://github.com/BokSIL-SEOB"><img src="https://avatars.githubusercontent.com/BokSIL-SEOB" width="130px;" height="130px" alt=""></a></td>
        <td align="center"><a href="https://github.com/bogwang159"><img src="https://avatars.githubusercontent.com/bogwang159" width="130px;" height="130px" alt=""></a></td>
    </tr>
    <tr>
        <td align="center"><a href="https://github.com/Hae-in"><b>Hae-in</b></a></td>
        <td align="center"><a href="https://https://github.com/seongsiyoung"><b>seongsiyoung</b></a></td>
        <td align="center"><a href="https://github.com/BokSIL-SEOB"><b>BokSIL-SEOB</b></a></td>
        <td align="center"><a href="https://github.com/bogwang159"><b>bogwang159</b></a></td>
    </tr>
    <tr>
        <td align="center"><a href="https://github.com/d4been"><img src="https://avatars.githubusercontent.com/d4been" width="130px;" height="130px" alt=""></a></td>
        <td align="center"><a href="https://github.com/yeongbeomSong"><img src="https://avatars.githubusercontent.com/yeongbeomSong" width="130px;" height="130px" alt=""></a></td>
        <td align="center"><a href="https://github.com/LGY77932"><img src="https://avatars.githubusercontent.com/LGY77932" width="130px;" height="130px" alt=""></a></td>
        <td align="center"><a href="https://github.com/Hirundo537"><img src="https://avatars.githubusercontent.com/Hirundo537" width="130px;" height="130px" alt=""></a></td>
    </tr>
    <tr>
        <td align="center"><a href="https://github.com/d4been-in"><b>d4been</b></a></td>
        <td align="center"><a href="https://https://github.com/yeongbeomSong"><b>yeongbeomSong</b></a></td>
        <td align="center"><a href="https://github.com/LGY77932"><b>LGY77932</b></a></td>
        <td align="center"><a href="https://github.com/Hirundo537"><b>Hirundo537</b></a></td>
    </tr>
</table>

## 🗂️ 문서

- [회고록 모음](./docs/retrospective)

## ⚙️ 기술 스택

- Java

---

## 미니 프로젝트 가이드

본 문서는 8명의 팀원이 각자 프로젝트를 독립적으로 진행하면서, 원활하게 협업하기 위한 가이드라인입니다.

---


## 1. 기본 협업 방식
- **팀 레포지토리**: `https://github.com/LikeLionTeam-2/miniproject.git`
- 각자 팀 레포지토리를 **포크(Fork)** 해서 본인 계정으로 복사합니다.
- 본인 계정에서 본인 이름의 브랜치를 생성해 작업 후, 팀 레포지토리로 **Pull Request(PR)** 를 생성합니다.


---

### 2.2 개인 브랜치 생성하기
- 브랜치 이름은 **본인 이름**으로 작성합니다.
```bash
git checkout -b 이름
```


예시:
```bash
git checkout -b Haein
```

- 생성한 브랜치 push
```
git push --set-upstream origin Haein
```

### 2.3 프로젝트 작성하기
- 자신의 디렉토리 외에는 수정하지 않습니다.


### 2.4 변경사항 커밋 & 푸시
```bash
git add .
git commit -m "[이름] 프로젝트 초기 설정"
git push origin 이름
```

### 2.5 팀 레포지토리로 Pull Request 생성
1. GitHub 개인 레포지토리 페이지로 이동합니다.
2. **Compare & Pull Request** 버튼 클릭.
3. Base Repository → 팀 레포지토리의 `main` 브랜치, Compare → 본인 브랜치로 설정.
4. 변경사항 설명 후 **Pull Request 생성**.


---


## 3. 팀 레포지토리 최신화하기 (Upstream 설정)
팀 저장소가 업데이트될 수 있으므로, 주기적으로 최신화해야 합니다.


1. 팀 저장소를 upstream 으로 등록:
```bash
git remote add upstream https://github.com/LikeLionTeam-2/miniproject.git
```


2. 최신 코드 가져오기:
```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```


---


## 4. 협업 규칙
- **본인 이름 디렉토리만 수정**.
- **브랜치명 = 본인 이름**.
- **Pull Request**는 본인이 작성한 내용만 포함.
- 다른 팀원의 코드는 직접 수정하지 말고, 필요하면 Issue로 논의.


---


## 5. 예시 워크플로우
```bash
# 레포지토리 클론
git clone https://github.com/내아이디/miniproject.git


# 브랜치 생성
git checkout -b Haein


# 작업 후 커밋 & 푸시
git add .
git commit -m "[Haein] 프로젝트 기능 추가"
git push origin kim


# GitHub에서 Pull Request 생성
```


---


## 6. 참고
- Git 공식 문서: [https://git-scm.com/doc](https://git-scm.com/doc)
- GitHub 협업 가이드: [https://docs.github.com](https://docs.github.com)
