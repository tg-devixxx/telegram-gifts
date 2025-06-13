## RU
Цены на подарки из Tonnel можно получи при помощи запроса:
```
async function getPrices() {
  try {
    const response = await fetch('https://raw.githubusercontent.com/tg-devixxx/telegram-gifts/main/tonnel-prices.json');
    
    if (!response.ok) throw new Error(`HTTP error! Status: ${response.status}`);
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Error fetching data:", error);
  }
}

getPrices();
```

По мере появляения времени, вохможно сделаю API. 

`✅ Обновление цен происходит раз в час, лучше всего обновлять свою бд этими записями.`

## ENG
Tonnel gift prices can be fetched using the following request:
```
async function getPrices() {
  try {
    const response = await fetch('https://raw.githubusercontent.com/tg-devixxx/telegram-gifts/main/tonnel-prices.json');
    
    if (!response.ok) throw new Error(`HTTP error! Status: ${response.status}`);
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Error fetching data:", error);
  }
}

getPrices();
```
I may add a full API later when time allows.  
`✅ Prices are updated every hour — it's recommended to sync your database with this file.`

