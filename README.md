## Кирилл Шишкин · Information Security

Студент 3 курса Финансового университета при Правительстве РФ, направление 10.03.01
«Безопасность автоматизированных систем в кредитно-финансовой сфере».

Занимаюсь информационной безопасностью с трёх сторон:

- 🔐 **Безопасная разработка.** Пишу защищённые приложения с нуля: модель угроз, криптография, автотесты на меры защиты, CodeQL / bandit / pip-audit / gitleaks в CI.
- 🛡️ **SOC и Detection Engineering.** Wazuh, Sysmon, Sigma, правила обнаружения с привязкой к MITRE ATT&CK.
- 🎯 **Пентест веб-приложений.** OWASP Top 10, Burp Suite, Kali Linux.

Участник Всероссийского квантового хакатона Quant-NN 2025 (9 место по РФ), соавтор публикации о защите данных в мессенджерах.

### ⭐ Главные проекты

#### [🌲 Лес из Шишек](https://github.com/ShishaKirich/grpc-messenger) — защищённый мессенджер
Мессенджер на gRPC (только TLS) с клиентом на PySide6 и личным кабинетом на FastAPI.
Сквозное шифрование X25519 + ChaCha20-Poly1305 с подписью Ed25519, секретные чаты на **X3DH и Double Ratchet** (как в Signal),
код безопасности для сверки ключей, двухфакторный вход (почта, TOTP, резервные коды).
78 автотестов, модель угроз в SECURITY.md, CI: CodeQL, bandit, pip-audit, gitleaks.

#### [🔑 2FA Auth Site](https://github.com/ShishaKirich/2fa-auth-site) — вход в два шага
Веб-сервис регистрации и входа: код на почту или TOTP по QR-коду, резервные коды, доверенные устройства,
активные сеансы. Argon2id, проверка паролей по HIBP, CSRF, строгий CSP, защита от перебора.
Нагрузочный тест: 300 одновременных пользователей, 0 ошибок. Ядро аутентификации перенесено в мессенджер.

#### [🛡️ Home SOC Lab](https://github.com/ShishaKirich/home-soc-lab) — домашний SOC-стенд
Wazuh SIEM + Sysmon, правила Wazuh и Sigma по MITRE ATT&CK с unit-тестами в CI (Detection-as-Code),
эмуляция атак Atomic Red Team, Suricata, детекты атак на Active Directory, SOAR (Shuffle + TheHive), ГОСТ Р 57580.1.

#### [🧃 OWASP Juice Shop](https://github.com/ShishaKirich/juice-shop-security-report) — анализ защищённости
Поиск, эксплуатация и устранение 49 уязвимостей: SQL/NoSQL-инъекции, XSS, IDOR, XXE, SSRF, JWT.
Покрыты все категории OWASP Top 10 2021, для каждой уязвимости исправление «было → стало».

### 🧰 Стек

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![gRPC](https://img.shields.io/badge/-gRPC-244c5a?style=flat&logo=google&logoColor=white)
![Qt](https://img.shields.io/badge/-PySide6%20(Qt)-41CD52?style=flat&logo=qt&logoColor=white)
![SQLite](https://img.shields.io/badge/-SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![CodeQL](https://img.shields.io/badge/-CodeQL-2F4F4F?style=flat&logo=github&logoColor=white)
![Wazuh](https://img.shields.io/badge/-Wazuh-005571?style=flat&logo=wazuh&logoColor=white)
![Kali Linux](https://img.shields.io/badge/-Kali%20Linux-557C94?style=flat&logo=kalilinux&logoColor=white)
![Burp Suite](https://img.shields.io/badge/-Burp%20Suite-FF6633?style=flat&logo=burpsuite&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat&logo=docker&logoColor=white)

**Криптография:** X25519, Ed25519, ChaCha20-Poly1305, X3DH, Double Ratchet, Argon2id, HMAC, TOTP, TLS со своим CA.

### 🧪 Другие проекты

<details>
<summary>Квантовые вычисления, оптимизация, автоматизация</summary>

| Проект | Описание |
|--------|----------|
| [RWA](https://github.com/ShishaKirich/RWA) | Маршрутизация и назначение длин волн в оптических сетях (квантовый хакатон, 9 место) |
| [quantum-state-2025](https://github.com/ShishaKirich/quantum-state-2025) | Квантовое состояние \|2025⟩ на 7 кубитах (Qiskit, OpenQASM) |
| [two-level-unitary-matrices](https://github.com/ShishaKirich/two-level-unitary-matrices) | Разложение унитарных матриц на двухуровневые операторы |
| [QUBO](https://github.com/ShishaKirich/QUBO) | Эвристический решатель задачи QUBO |
| [check-news](https://github.com/ShishaKirich/check-news) | UI-автотесты на Selenium + pytest |
| [GSPOM](https://github.com/ShishaKirich/GSPOM) | Голосовой ассистент «Скай» |

</details>
