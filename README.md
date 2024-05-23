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
- 로그인 페이지 Animated를 통해 사용자 친화적인 UI 제공 (Signin, Signup) -> `삼항 연산자`를 통해 Login과 Signup일때 UI 변환 -> `Authentication`
- 비동기 방식의 메소드
- Stream과 파이어베이스

![123](https://github.com/shyang12/chatting_app/assets/85710913/92ac2e2e-3dcd-4515-80b8-587f21ece0fb)

- 로그인 페이지 Signup 옆 프로필 사진 지정 가능한 위젯 -> `Storage`
- `Firebase 규칙` 수정을 통해 제 3자가 데이터를 수정, 조회, 생성하는 일을 방지
- ChatBubble을 사용한 채팅창 UI 개선 -> `삼항 연산자`를 통해 내 채팅, 상대방 채팅 (왼쪽, 오른쪽) UI 구성 -> `Firestore Database` + `Storage`
- 정렬 `Descending`을 통해 `TimeStamp`순으로 채팅방 정렬 -> `Firestore Database`
- 내 채팅의 이름, 상대 채팅의 이름, 나와 상대방의 프로필 사진 UI 개선 -> `Storage`
  
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
### 3.1 Authentication

### 3.2 Firestore Database
```bash
├── chats
│    └── message
├── chat
│    ├── text
│    ├── time
│    ├── userID
│    ├── userImage
│    └── userName
├── user
│    ├── email
│    ├── picked_image
│    └── userName
```

### 3.3 Firebase Storage
```bash
├── picked_images
│    └── ~~~.PNG
```

## 4. Result
- 로그인 화면 (Login, Signup)

![로그인](https://github.com/shyang12/chatting_app/assets/85710913/4c280c4a-c592-4a80-b1fc-f853e65ac773)  ![로그인 사인업](https://github.com/shyang12/chatting_app/assets/85710913/41c4e299-c21e-4645-b956-6263e652bee3)


- 회원가입에 이미지 저장 및 사진 촬영

![이미지 저장](https://github.com/shyang12/chatting_app/assets/85710913/1bb3db6d-7e0b-4f07-81db-e6fd5094a9e0)  ![사진촬영](https://github.com/shyang12/chatting_app/assets/85710913/d91df66f-3794-48c3-98e0-9968c806b78b)


- 채팅방 채팅 내용

![채팅](https://github.com/shyang12/chatting_app/assets/85710913/193d97d4-5380-4177-8002-72cf68924483)  ![채팅방 2](https://github.com/shyang12/chatting_app/assets/85710913/b7bb62f1-66b9-45d0-9f03-ede868a19d8e)

