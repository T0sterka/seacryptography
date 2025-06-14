```markdown
# 🔐 Telegram Encryption Bot

Многофункциональный бот для криптографических операций с удобным Telegram-интерфейсом.

## 🌟 Основные функции

### 🔐 Шифрование данных
```python
# Пример AES-шифрования
fernet = Fernet(key.encode())
encrypted = fernet.encrypt(text.encode())
```

### 🔑 Генерация ключей
- RSA ключи 2048 бит
- Автоматические AES ключи

### 🔢 Генератор паролей
```python
# Генерация сложного пароля
password = ''.join(secrets.choice(string.ascii_letters + string.digits + string.punctuation) for _ in range(16))
```

### ⚠ Проверка утечек
```python
# Проверка пароля через HIBP API
sha1_hash = hashlib.sha1(password.encode()).hexdigest().upper()
```

## 🛠 Технологический стек

| Технология         | Назначение                     |
|--------------------|--------------------------------|
| Python 3.10+       | Основной язык                  |
| pyTelegramBotAPI   | Работа с Telegram API          |
| cryptography       | Криптографические операции     |
| requests           | Работа с API проверки утечек   |

## ⚙ Установка и запуск

1. Установите зависимости:
```bash
pip install -r requirements.txt
```

2. Создайте файл конфигурации `config.py`:
```python
TOKEN = 'ваш_telegram_токен'
HIBP_API_KEY = 'ваш_api_ключ_haveibeenpwned'
```

3. Запустите бота:
```bash
python bot.py
```

## 📊 Структура проекта

```
/telegram-encryption-bot
│
├── bot.py            # Основной код бота
├── config.py         # Конфигурационные данные
├── requirements.txt  # Зависимости
└── README.md         # Документация
```
