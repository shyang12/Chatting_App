# Chatting_app
## ▶ 안드로이드 스튜디오 채팅앱 만들기 (Flutter -> dart)
 
 - 안드로이드 스튜디오에서 Flutter(dart)를 기반으로 채팅 앱을 구현하는 프로젝트

`Stream` `Firebase` `Authentication` `Firestore Database` `Storage` `flutter_chat_bubble` `modal_progress_hud` `image_picker`

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
- 로그인 페이지 Animated를 통해 사용자 친화적인 UI 제공 (Signin, Signup) -> `삼항 연산자`를 통해 Login과 Signup일때 UI 변환  `Authentication
- 비동기 방식의 메소드
- Stream과 파이어베이스

![123](https://github.com/shyang12/chatting_app/assets/85710913/92ac2e2e-3dcd-4515-80b8-587f21ece0fb)

- 로그인 페이지 Signup 옆 프로필 사진 지정 가능한 위젯  `Storage`
- `Firebase 규칙` 수정을 통해 제 3자가 데이터를 수정, 조회, 생성하는 일을 방지
- ChatBubble을 사용한 채팅창 UI 개선 -> `삼항 연산자`를 통해 내 채팅, 상대방 채팅 (왼쪽, 오른쪽) UI 구성 `Firestore Database` + `Storage`
- 정렬 `Descending`을 통해 `TimeStamp`순으로 채팅방 정렬  `Firestore Database`
- 내 채팅의 이름, 상대 채팅의 이름, 나와 상대방의 프로필 사진 UI 개선 `Storage`
  
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
├── chat
│   ├── chat_bubble.dart
│   ├── message.dart
│   └── new_message.dart
├── add_image
│   └── add_image.dart
```

## 3. Firebase   
### 3.1 Firestore Database
```bash
├── chats
│    └── message
├── chat
│    ├── text
│    ├── time
│    ├── userID
│    └── userName
├── user
│    ├── email
│    └── userName
```

## 4. Result
- 로그인 화면

![로그인](https://github.com/shyang12/chatting_app/assets/85710913/9fcafca8-9c02-41ac-8a97-d9c353431048)
