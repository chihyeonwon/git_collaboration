# git_collaboration
[Git] 깃 협업 정리
```
내가 하는 협업 프로세스와 유사한 것 같아서 정리한 것을 가져왔다.

1. 팀장이 개발 환경이나 gitignore같은 환경설정을 한다음 프로젝트를 생성
2. 레포지토리 파서 프로젝트를 업로드push
3. 팀원은 팀장의 레포지토리를 fork
4. 팀원은 팀장의 레포지토리를 clone 해서 로컬로 받아온다음 실행여부 확인
5. 실행이 잘되면 로컬에서 작업한 다음 개개인의 브랜치에 push하면서 작업
6. 팀장한테 push하고자할 때는 PR pull request를 보낸다.
```
![image](https://github.com/chihyeonwon/git_collaboration/assets/58906858/2121aa05-4afc-4e38-ab5d-f2ebef3a7086)
![image](https://github.com/chihyeonwon/git_collaboration/assets/58906858/31c6f37d-bfad-4af9-beb2-0804ea1a3cda)

```
팀장 브랜치와 <> 나의 브랜치를 비교해서 pull request를 보내면 able to merge가 뜨면
진행
```

## 단 Merge시 Conflict 발생
![image](https://github.com/chihyeonwon/git_collaboration/assets/58906858/c91160b2-321f-47f7-9df9-ff82c6f34b9d)
```
Conflict 발생 시 automatically merge 빨간색으로 뜬다.

```
![image](https://github.com/chihyeonwon/git_collaboration/assets/58906858/f254eca1-72e1-412b-9f26-97b7196277ab)
```
팀장의 레포를 팀원의 레포로 pull로 받아온다음 conlict 나는 부분을 수정한 후 다시 push 한다음 팀장에 PR 보낸다.

Conflict 발생 이유 : 팀장의 최신 프로젝트를 pull로 가져오지 먼저 가져오지 않았기 때문에 발생
```
## 여러 명과 협업 시
![image](https://github.com/chihyeonwon/git_collaboration/assets/58906858/eb119efa-668c-4ee0-8168-81aee9040b84)
```
순차적으로 진행 1번 로컬에서 Conflict 해결 후 팀장으로 pr보내고 팀장은 1번에 대한 수정사항을 merge 한다. 2번은 다시 팀장의 프로젝트를 pull로 가져간다음 Conflict 해결 후 팀장으로 pr
팀장은 2번에 대한 수정사항을 merge 즉 순차적으로 진행 (아주 복잡)
```

