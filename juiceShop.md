## Контрольная работа №2
*Студент Гуцалюк Д.Ю. группа УИБО-02-24*

## Задание 1
### Использованные данные:
*Login:* ' or 1=1;--

*Password:* 123

### Пользователь:
Удалось войти как: admin@juice-sh.op

### Почему удалось войти:
SQL-инъекция изменила запрос, условие стало TRUE (`1=1`) и сервер вернул первую запись в таблице пользователей.

### Где хранится аутентификация:
После выполнения SQL-инъекции в браузере появляется токен аутентификации.
Тип: JWT токен (JSON Web Token)
Структура: header.payload.signature (3 части)
Кодировка: Base64URL
Назначение: передаёт данные о пользователе + подтверждает сессию
Хранится в разделе Cookies и в Local storage:
Имя: token
Cookie: token=eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJzdGF0dXMiOiJzdWNjZXNzIiwiZGF0YSI6eyJpZCI6MSwidXNlcm5hbWUiOiIiLCJlbWFpbCI6ImFkbWluQGp1aWNlLXNoLm9wIiwicGFzc3dvcmQiOiIwMTkyMDIzYTdiYmQ3MzI1MDUxNmYwNjlkZjE4YjUwMCIsInJvbGUiOiJhZG1pbiIsImRlbHV4ZVRva2VuIjoiIiwibGFzdExvZ2luSXAiOiIiLCJwcm9maWxlSW1hZ2UiOiJhc3NldHMvcHVibGljL2ltYWdlcy91cGxvYWRzL2RlZmF1bHRBZG1pbi5wbmciLCJ0b3RwU2VjcmV0IjoiIiwiaXNBY3RpdmUiOnRydWUsImNyZWF0ZWRBdCI6IjIwMjUtMTEtMTYgMjA6MDI6MDYuMDQ0ICswMDowMCIsInVwZGF0ZWRBdCI6IjIwMjUtMTEtMTYgMjA6MDI6MDYuMDQ0ICswMDowMCIsImRlbGV0ZWRBdCI6bnVsbH0sImlhdCI6MTc2MzMyMzg3M30.sNQjqDgT_XKWfRYIEOTMyTdP33DjNz1A_M0LvGMs_R3YN_oT35acYq_dX4bSogqh9IJnCH3MbDflNvkOpSTDRe20maf1iSng36cnh2vBDIBqNK0xm5aD8hID7OXUXSD-EGlV_9e_oynQRC8DF16rupb9Lam2gVmcnX6IKistjsM

### Скриншоты:
<img width="755" height="639" alt="{B54F545A-D37A-4138-88CC-76595C9CFAD7}" src="https://github.com/user-attachments/assets/d942cfe1-8f43-4b0c-9dee-4af6c56b4a05" />
<img width="1124" height="648" alt="image" src="https://github.com/user-attachments/assets/b8330d7a-17cc-4f78-9202-8c0e370d5a2c" />

## Задание 2
