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
1. Klonowanie repozytorium:

   ```sh
   git clone https://github.com/marder/myWeatherAppFull.git
    ```

2. Instalacja i uruchomienie sewera back-endowego w trybie deweloperskim:

   ```sh
   cd Backend
   npm install
   npm run dev
    ```

3. Instalacja i uruchomienie front-endu w trybie deweloperskim:

   ```sh
   cd Frontend
   npm install
   npm run dev
    ```

4. Przygotowanie front-endu do publikacji:

   ```sh
   cd Frontend
   npm run build
    ```

5. W katalogu Device znajduje się kod przygotowany dla Arduino MKR WiFi 1010 wraz z czujnikiem BME280. Wymagane jest utworzenie pliku arduino_secrets.h zawierającego nazwę Wi-Fi (SSID), hasła oraz adresu serwera back-girt endowego.

# Uwaga

Niniejsze repozytorium zostało opublikowane dla dociekliwych pasjonatów, którzy w miarę kumają kod i chieliby w niego zerknąć. Zdaję sobie sprawę, że powyższy opis nie stanowi dokumentacji, a jedynie zarys opisu projektu i wymaga on uszczegółowienia.