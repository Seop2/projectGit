# 자주 쓰는 Git 명령어 정리

## 저장소 초기화

```bash
git init
```

## 원격 저장소 연결

```bash
git remote add origin <원격저장소URL>
```

## 변경 사항 확인

```bash
git status
```

## 파일 스테이징

```bash
git add <파일명>
git add .
```

## 커밋 생성

```bash
git commit -m "커밋 메시지"
```

## 브랜치 목록 확인 및 생성

```bash
git branch
git branch <브랜치명>
```

## 브랜치 이동

```bash
git checkout <브랜치명>
```

## 브랜치 생성과 이동

```bash
git checkout -b <브랜치명>
```

## 원격 저장소에서 변경 사항 가져오기

```bash
git pull
```

## 변경 사항 원격 저장소에 반영

```bash
git push
```

## 로그 확인

```bash
git log
```

## 코드리뷰 요청 및 반영

### Pull Request(PR) 생성

GitHub, GitLab 등에서 브랜치를 푸시한 후 웹에서 PR을 생성합니다.

### PR 관련 명령어

```bash
# PR 대상 브랜치로 이동
git checkout <feature-branch>

# 변경 사항 푸시
git push origin <feature-branch>
```

### 코드리뷰 반영 후

```bash
# 리뷰 반영 후 커밋
git add <수정파일>
git commit -m "리뷰 반영: <내용>"
git push origin <feature-branch>
```
