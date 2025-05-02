# myWeatherApp ☀️🌧️

Projekt myWeatherApp – czyli jak z czujnika i hektolitrów kawy zrobić pogodowego potwora!

## 📖 O projekcie
Dawno, dawno temu (czyli w 2021 roku), w krainie kodu i niekończących się tutoriali, narodził się pomysł stworzenia inteligentnej stacji pogodowej. Zaczęło się od Arduino, kilku czujników środowiskowych i idei „Zróbmy coś, co pokazuje temperaturę i nie wybucha”.

Tak powstał **myWeatherApp**, czyli aplikacja do monitorowania warunków atmosferycznych i wizualizacji danych pogodowych.

## 🛠️ Technologie i komponenty

### Klient (hardware)
- **Arduino MKR WiFi 1010**
- **Nakładka MKR IoT Carrier**
- **Czujnik BME280 (Grove)**
- **Zasilanie**: bateria 18650 Li-Ion 3.7V + powerbank

### Backend
- **Node.js + ExpressJS**
- **REST API**
- **Baza danych MongoDB**

### Frontend
- **VueJS 3**
- **TailwindCSS**
- **ChartJS** – wizualizacja danych pogodowych

### Hosting
- **VPS od Mikr.us**
- **Ubuntu**
- **Nginx**

## 📊 Funkcjonalności
- Pobieranie danych pogodowych z czujników
- Przesyłanie danych do backendu przez Wi-Fi
- Wizualizacja danych w formie wykresów w aplikacji webowej
- Integracja z MongoDB dla przechowywania odczytów

## 🚀 Jak uruchomić?
1. Sklonuj repozytorium:
   ```sh
   git clone https://github.com/yourusername/myWeatherApp.git
    ```