# Currency Converter App 🌍💱

A simple React-based currency converter that allows users to convert amounts between different currencies using live exchange rates from [Fawaz Ahmed's Currency API](https://github.com/fawazahmed0/currency-api).

## 🚀 Features

* Real-time currency conversion using external API.
* Swap between source and target currencies with one click.
* Clean and responsive UI with Tailwind CSS.
* Custom `useCurrencyInfo` hook to fetch and manage exchange rates.
* Reusable `InputBox` component for currency input and selection.

## 🛠️ Tech Stack

* **React** (functional components + hooks)
* **Tailwind CSS** for styling
* **Fetch API** for data fetching

## 📂 Project Structure

```
src/
 ├── App.js             # Main app component
 ├── components/
 │    └── InputBox.js   # Reusable input + select box component
 ├── hooks/
 │    └── useCurrencyInfo.js  # Custom hook to fetch currency info
 ├── App.css
 └── index.js
```

## ⚙️ How to Run

1️⃣ Clone the repository:

```bash
git clone <your-repo-url>
cd <project-folder>
```

2️⃣ Install dependencies:

```bash
npm install
```

3️⃣ Run the app:

```bash
npm run dev  # If using Vite
# or
npm start    # If using CRA
```

4️⃣ Open [http://localhost:3000](http://localhost:3000) (or the port your dev server shows).

## ✨ How It Works

* The app initializes with default currencies: `USD` (from) and `INR` (to).
* Exchange rates for the `from` currency are fetched using the `useCurrencyInfo` hook.
* Users can enter an amount and select currencies to convert.
* Clicking **Convert** performs the conversion.
* The **Swap** button swaps the `from` and `to` currencies.

## 📌 API Used

[https://github.com/fawazahmed0/currency-api](https://github.com/fawazahmed0/currency-api)

Example API endpoint:

```
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/usd.json
```

## 📝 Notes

* The app prevents negative amounts.
* Conversion requires the API data to load; otherwise, the result will be `0`.
* The UI features a background image and a blur effect for enhanced aesthetics.

##
