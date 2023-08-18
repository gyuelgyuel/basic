
> 리눅스 명령어들을 정리

- `pwd` (present working directory)
    - 현재 작업중인 경로를 출력
- `ls` (list)
    - 현재 폴더에 있는 파일, 폴더를 출력
    - `-a` (optional) : 숨김처리된 파일, 폴더까지 출력
    - `-l` (optional) : 파일의 형태(r/w), 최근 수정 시간 출력
    - `-al` (optional) : `-a`, `-l` 둘다 수행
- `cd` (change directory)
    - 폴더 이동
- `mkdir` (make directory)
    - 폴더 생성
- `touch`
    - 파일 생성
- `rm` (remove)
    - 파일 삭제
    - `-r` (recursion)(optional) : 폴더 삭제
- `cp` (copy)
    - 파일 복사 : `cp <origin_file> <copy_file>`
- `mv` (move)
    - 이름 변경, 파일 이동 : `mv <origin_file> path/<rename_file>`
- `vi`
    - 파일 에디터로 보기
    - `i` : 수정, `:w` : 저장, `:q` : 종료
- `ctrl/shift + insert`
    - 복사/붙여넣기
- `code <file_name>`
    - VScode로 파일 열기