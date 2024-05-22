# Chatting_app
## ▶ 안드로이드 스튜디오 채팅앱 만들기 (Flutter -> dart)
 
 - 안드로이드 스튜디오에서 Flutter(dart)를 기반으로 채팅 앱을 구현하는 프로젝트

`kpostal (우편주소 API)` `Firebase` `Authentication` `Firestore Database`

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
- 상품 리스트를 ScrollView를 통해 상품 사진, 상품명, 가격등 정보 제공 -> `나의 주문목록, 장바구니 확인 버튼 위에 추가`
- 제품의 상세 페이지를 통해 제품의 상세 내용 제공
- 장바구니 기능을 통해 상품 개수 추가 or 감소, 삭제등 구매하기 전 장바구니 기능
- 우편번호(주소) API를 사용하여 사용자에게 택배 보낼 주소 저장 기능
- 주문목록에서 주문날짜, 주분정보, 주문취소, 배송조회등의 기능
- 주문완료 페이지를 통해 최종 결제

## 2. Project Architecture   
```bash
├── main
│   ├── main.dart
│   └── constants.dart
├── config
│   └── Palette.dart
├── screens
│   ├── main_screen.dart
├── enums
│   ├── delivery_status.dart
│   └── payment_status.dart
```

## 3. Firebase   
### 3.1 Firestore Database
```bash
├── orders
│    ├── buyerEmail
│    ├── buyerName
│    ├── buyerPhone
│    ├── deliveryStatus
│    ├── orderDate
│    ├── orderNo
│    ├── paymentMethod
│    ├── paymentStatus
│    ├── productNo
│    ├── quantity
│    ├── receiverAddress1
│    ├── receiverAddress2
│    ├── receiverName
│    ├── receiverPhone
│    ├── receiverZip
│    ├── totalPrice
│    ├── unitPrice
│    └── userPwd
├── products
│    ├── price
│    ├── productImageUrl
│    ├── productName
│    └── productNo
```

## 4. Result
- 로그인 화면

![로그인](https://github.com/shyang12/chatting_app/assets/85710913/9fcafca8-9c02-41ac-8a97-d9c353431048)
