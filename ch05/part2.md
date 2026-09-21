<img width="364" height="474" alt="image" src="https://github.com/user-attachments/assets/0ce1747f-cca2-44d0-883b-dfa06fee359e" />
<img width="447" height="741" alt="image" src="https://github.com/user-attachments/assets/d93579f6-855d-4719-9d7d-d5cc788e730e" />
<img width="248" height="875" alt="image" src="https://github.com/user-attachments/assets/9192df9c-322b-4e98-889d-5d4179781c06" />
 
| 구분 | 하드 링크 | 심볼릭 링크 |
|---|---|---|
| 생성 | `ln 원본 링크` | `ln -s 원본 링크` |
| 관계 | 같은 파일에 여러 이름 | 원본을 가리키는 별도 파일 |
| 원본 삭제 | 다른 하드 링크로 접근 가능 | 링크가 깨짐 |
| 디렉터리 링크 | 불가능 | 가능 |
| 다른 디스크 간 링크 | 불가능 | 가능 |
| 확인 | `ls -l`, inode 등 | `ls -l`에서 `->`로 확인 |

ls -l은 현재 디렉터리의 파일과 디렉터리 정보를 자세하게 출력하는 명령어이다. 심볼릭 링크가 존재하는 경우 파일 종류가 l로 표시되며, -> 기호 뒤에 해당 심볼릭 링크가 연결되어 있는 원본 파일이 표시된다.

<img width="399" height="97" alt="image" src="https://github.com/user-attachments/assets/c998a6e3-f91c-4692-9fad-cb2fb02bf615" />

디렉터리를 생성하면 내부에 기본적으로 . , .. 두 개의 디렉터리 항목이 생성된다. 
반면 일반 파일은 생성했을 때 자기 자신에 대한 이름 하나만 있으므로 하드 링크 수가 1개 임.
