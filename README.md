🔐 Telegram Encryption Bot
Телеграм-бот для шифрования данных, генерации паролей и проверки утечек.

📌 Возможности
🔐 AES-шифрование:

Шифрование и дешифрование текста с использованием алгоритма AES

Автоматическая генерация ключей

🔑 RSA-шифрование:

Генерация пары RSA-ключей (публичный/приватный)

Шифрование и дешифрование текста с помощью RSA

🔢 Генератор паролей:

Создание паролей разной сложности (8/12/16 символов)

Использование букв, цифр и специальных символов

⚠ Проверка утечек:

Проверка паролей через сервис Have I Been Pwned

Проверка email на наличие в известных утечках данных

🛠 Технологии
Python 3

Библиотека pyTelegramBotAPI

Криптографические библиотеки cryptography и hashlib

API Have I Been Pwned

⚙ Установка
Клонируйте репозиторий:

bash
git clone https://github.com/ваш-username/telegram-encryption-bot.git
cd telegram-encryption-bot
Установите зависимости:

bash
pip install -r requirements.txt
Создайте файл config.py и добавьте ваш Telegram токен:

python
TOKEN = 'ваш_telegram_токен'
HIBP_API_KEY = 'ваш_api_ключ_haveibeenpwned'
Запустите бота:

bash
python bot.py
📝 Лицензия
Этот проект распространяется под лицензией MIT. Подробнее см. в файле LICENSE.
