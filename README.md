# 🏨 Hotel Reservation System (Java)

Bu proje, bir otelin oda yönetimi ve rezervasyon süreçlerini yönetmek amacıyla geliştirilmiş **Java tabanlı bir otel rezervasyon sistemidir**.

Sistem; oda yönetimi, müşteri bilgileri ve rezervasyon işlemlerini yönetmek için **katmanlı mimari yaklaşımı** kullanılarak tasarlanmıştır. Uygulama **konsol tabanlı bir kullanıcı arayüzü** üzerinden çalışmaktadır.

---

# 🚀 Features

- 🏨 Oda ekleme ve listeleme
- 📅 Rezervasyon oluşturma
- ❌ Rezervasyon iptal etme
- 👤 Müşteri bilgilerini yönetme
- 💾 Verileri dosya tabanlı saklama
- 🔎 Veri doğrulama ve tarih kontrolü

---

# 🛠 Tech Stack

| Teknoloji | Açıklama |
|-----------|----------|
| Java | Ana programlama dili |
| Maven | Proje yönetimi (opsiyonel) |
| File Storage | rooms.txt ve reservations.txt ile veri saklama |
| JUnit | Birim testleri |

---

# 📂 Project Structure

hotel-reservation-system
│
├── Main.java
├── ConsoleUI.java
│
├── models
│ ├── Room.java
│ ├── Reservation.java
│ └── Customer.java
│
├── controllers
│ ├── ReservationController.java
│ ├── RoomController.java
│ └── CustomerController.java
│
├── services
│ ├── ReservationManager.java
│ └── RoomManager.java
│
├── database
│ └── Database.java
│
├── utils
│ ├── DateUtils.java
│ └── Validator.java
│
├── data
│ ├── rooms.txt
│ └── reservations.txt
│
├── tests
│ ├── TestReservationManager.java
│ └── TestRoomManager.java
│
├── run.sh
├── run.bat
└── pom.xml


---

# 🧱 System Architecture

Proje **katmanlı mimari** kullanılarak geliştirilmiştir.

### Model Layer
Sistemdeki veri yapıları.

- `Room.java`
- `Reservation.java`
- `Customer.java`

### Controller Layer
Kullanıcıdan gelen işlemleri yönetir ve servis katmanına yönlendirir.

- `ReservationController`
- `RoomController`
- `CustomerController`

### Service Layer
İş mantığını içerir.

- `ReservationManager`
- `RoomManager`

### Data Layer
Veri okuma ve yazma işlemlerini gerçekleştirir.

- `Database.java`

---

# 💾 Data Storage

Sistem verileri **metin dosyalarında saklanmaktadır**.

### rooms.txt
Oda bilgileri:

RoomNumber,RoomType,Price


### reservations.txt
Rezervasyon bilgileri:

CustomerName,RoomNumber,CheckInDate,CheckOutDate


---

# 🧪 Unit Tests

Projede bazı işlevleri doğrulamak için birim testleri bulunmaktadır.

- `TestReservationManager.java`
- `TestRoomManager.java`

---

# 🚦 Installation & Run

### 1️⃣ Repoyu klonlayın

git clone https://github.com/username/hotel-reservation-system.git


### 2️⃣ Proje klasörüne girin

cd hotel-reservation-system


### 3️⃣ Programı çalıştırın

Windows:

run.bat


Linux / Mac:

./run.sh


veya manuel olarak:

javac Main.java
java Main


---

# 📝 Notes

- Sistem **konsol tabanlıdır**.
- Veriler **dosya tabanlı veri depolama** yöntemi ile saklanır.
- Tarih doğrulama ve veri kontrolü için yardımcı sınıflar kullanılmıştır.

---
