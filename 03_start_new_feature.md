# 새로운 기능 개발 시작

## Fork 

* https://github.com/lim-dongsun/git_practice

* [repo init 은 readme 파일 참고](./01_readme.md)

## 기능 단위 브랜치 생성

```bash
git branch feature/add-profile
git checkout feature/add-profile
```

### 확인

```bash
git log --graph --all --oneline
```

OR

```bash
git log --graph --simplify-by-decoration --pretty=format:'%d' --all
```

OR

![003](/Users/1004790/workspace/git_practice/image/003.png)

### Branch 란?

![005](/Users/1004790/workspace/git_practice/image/005.png)

* Branch : 가지, 분기

* 이해하기 쉽게 생각하면 평행세계
  ![006](/Users/1004790/workspace/git_practice/image/006.jpg)



## 기능 개발 중 변경사항 저장

```bash
echo "# profile" >> profile.md
git add .
git commit -m "add profile file"
git push origin feature/add-profile
```

## 코드 리뷰, 병합

* 팀원이 올린 PR(Pull Request)을 검토하고 병합 

  ```bash
  git merge feature/add-profile
  ```

  
