### 설치
```bash
pip install fastapi
```
프로덕션을 위해 Uvicorn 또는 Hypercorn과 같은 ASGI 서버도 필요
```bash
pip install "uvicorn[standard]"
```

### 실행
```bash
uvicorn main:app --reload
```
테스트
```bash
http://127.0.0.1:8000/items/5?q=somequery
```
응답 데이터
```bash
{"item_id": 5, "q": "somequery"}
```
### API 문서
```bash
http://127.0.0.1:8000/docs

http://127.0.0.1:8000/redoc
```