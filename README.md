# Chatting_app
## ▶ 안드로이드 스튜디오 채팅앱 만들기 (Flutter -> dart)
 
 - 안드로이드 스튜디오에서 Flutter(dart)를 기반으로 채팅 앱을 구현하는 프로젝트

`Stream` `Firebase` `Authentication` `Firestore Database`

## 1. Co-Development Environment   
### 1. 1 Environments
- Windows 10
- Android Studio / Flutter / Dart
- Firebase
- GitHub

### 1. 2 Driving
- Android
- IOS
- WEB
- Window

### 1. 3 Implement
- 로그인 페이지 Animated를 통해 사용자 친화적인 UI 제공 (Signin, Signup) -> `삼항 연산자`를 통해 Login과 Signup일때 UI 변환
- 빙동기 방식의 메소드
- Stream과 파이어베이스

![123](https://github.com/shyang12/chatting_app/assets/85710913/92ac2e2e-3dcd-4515-80b8-587f21ece0fb)

- 
  
## 2. Project Architecture   
```bash
├── main
│   ├── main.dart
│   └── constants.dart
├── config
│   └── Palette.dart
├── screens
│   ├── main_screen.dart
│   └── chat_screen.dart
```

## 3. Firebase   
### 3.1 Firestore Database
```bash
├── chats
│    └── message
│    │    ├── buyerName
│    │    └── userPwd
├── products
│    ├── price
│    ├── productImageUrl
│    ├── productName
│    └── productNo
```

## 4. Result
- 로그인 화면

![로그인](https://github.com/shyang12/chatting_app/assets/85710913/9fcafca8-9c02-41ac-8a97-d9c353431048)
