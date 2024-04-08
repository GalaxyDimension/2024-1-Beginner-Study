#### Git log
+ commit 기록을 최신 순으로 확인
+ --Oneline 옵션을 사용하면 각 커밋을 한 줄에 요약

#### Head
+ 현재 작업중인 위치를 가리킨다.
+ 현재 작업중인 Branch의 최신 commit
+ 다음 commit의 base가 되는 commit
+ 새로운 commit이 생기면 Head도 변경

#### commit --amend
+ 마지막 commit 내용 변경시 사용
+ 완전히 새로운 commit으로 대체(commit id가 변경됨)
+ vim으로 진입하여 수정하게 됨
+ vim 진입이 싫으면 git commit --amend -m "내용"
+ commit 메시지 없이 수정 git commit --amend --no-edit

+ 다른사람이 작업중인 commit은 amend를 사용하면 안됨

#### reset
+ soft
  + reset --soft
  + commit만 취소
  + stage area로 변경사항이 돌아감

+ mixed
  + reset --mixed
  + default 값
  + commit을 취소
  + working area로 변경사항이 돌아감

+ hard
  + reset --hard
  + commit을 취소
  + 변경사항을 모두 제거 후 이전 commit으로 돌아감

#### revert
+ commit을 제거하지 않고 되돌림
+ 되돌리기 위하여 새로운 commit 생성
+ 편집기 없이 바로 git revert --no-edit "commit id"
+ commit 없이 staging area로 revert --no-commit

+ reset보다 revert가 안전
