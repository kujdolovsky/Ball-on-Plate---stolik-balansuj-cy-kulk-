# 🔧 Stolik balansujący kulką (Ball on Plate)

## 📌 Opis
Projekt układu sterowania stolikiem balansującym kulką z wykorzystaniem manipulatora 3RRS, regulatora PID oraz mikrokontrolera Arduino UNO.  
Celem było stabilizowanie kulki w zadanym punkcie oraz realizacja prostych trajektorii ruchu.

<img width="300" src="https://github.com/user-attachments/assets/5a16e375-8e2b-4d3b-a7fc-4d6dcec1f0aa" />

---

## 🎯 Cel projektu
- stabilizacja kulki w punkcie (0,0)
- implementacja regulatora PID w dwóch osiach
- realizacja trajektorii (okrąg, kwadrat)
- implementacja algorytmu na rzeczywistym układzie

---

## 🛠️ Narzędzia
- Matlab / Simulink
- Arduino IDE (C++)
- Filtracja sygnału (FIR)

---

## 🧠 Co zrobiłem
- opracowałem model matematyczny układu
- dobrałem nastawy regulatora PID
- zaimplementowałem sterowanie silnikami krokowymi
- napisałem algorytm odczytu pozycji kulki
- zaprojektowałem filtr FIR do przetwarzania sygnału
- przeanalizowałem możliwość zastosowania regulatora ADRC

---

## 📊 Wyniki

### Odpowiedź skokowa
- czas regulacji: ~2 s dla skoku 25 mm
- test dla przejścia z (25,25) → (0,0)

<img width="400" src="https://github.com/user-attachments/assets/6be00de1-8fcb-4ea3-a438-ef2cae340720" />

---

### Odporność na zakłócenia
- układ stabilizuje kulkę po zaburzeniu (pchnięcie)

<img width="400" src="https://github.com/user-attachments/assets/662a6bfb-986c-46cd-9281-b41ddc3d0b15" />

---

### Trajektorie ruchu
- poprawna realizacja ruchu po okręgu i kwadracie
- zgodność z wartością zadaną

<img width="300" src="https://github.com/user-attachments/assets/6d6e8734-25c3-461f-b381-3cc0a7beb066" />

---

## 🌀 Demo wideo (kliknij, aby obejrzeć)
Układ stabilizuje kulkę, kompensuje zakłócenia oraz realizuje zadane trajektorie ruchu.

### Reakcja na zakłócenia
[![Demo](https://img.youtube.com/vi/wO5LeluoGk4/0.jpg)](https://www.youtube.com/watch?v=wO5LeluoGk4)

### Trajektoria Prostokąta
[![Trajektoria](https://img.youtube.com/vi/QgTJa6kDOz0/0.jpg)](https://www.youtube.com/watch?v=QgTJa6kDOz0)

### Trajektoria koła
[![Zakłócenia](https://img.youtube.com/vi/Sv3K1zqYGdE/0.jpg)](https://www.youtube.com/watch?v=Sv3K1zqYGdE)



---

## 📉 Ograniczenia
- odchyłka statyczna do ~5 mm w stanie ustalonym

---

## 📄 Raport
[Pełny raport PDF](./raport.pdf)
