# Интеллектуальная платформа для верификации мультимедийного контента

## Краткое описание проекта

Платформа обеспечивает верификацию фото-, аудио- и видеоконтента в реальном времени с использованием технологий машинного обучения и блокчейна. Решение ориентировано на СМИ, социальные сети, государственные структуры и частные компании, сталкивающиеся с проблемой дезинформации.

**Ключевые возможности:**
- Потоковый анализ видео в реальном времени
- Детекция дипфейков и фейкового контента
- Блокчейн-логирование результатов верификации
- REST API для интеграции с внешними системами

## Техническое задание
[ТЗ проекта](./docs/ТПИС_Лаб2.pdf)

## Сборка и запуск проекта

### Предварительные требования
- Docker 20.10+
- Docker Compose 2.0+
- Python 3.9+
- Node.js 16+

### Технологический стек
- Backend: FastAPI, Python 3.9+
- Frontend: React, TypeScript
- AI/ML: PyTorch, TensorFlow, OpenCV
- Базы данных: PostgreSQL, Neo4j, S3-совместимое хранилище
- Блокчейн: Hyperledger Fabric
- Инфраструктура: Docker, Kubernetes, Nginx
- Очереди: RabbitMQ/Kafka

### Code Style
- Python: PEP8, Black, isort
- JavaScript: ESLint, Prettier
- Коммиты: Conventional Commits

### Локальная разработка
```bash
# Клонирование репозитория
git clone https://github.com/Mephistopheler/intelligent-media-verification-platform.git
cd intelligent-media-verification-platform

# Запуск сервисов
cd config
docker-compose up -d

# Установка зависимостей
pip install -r requirements.txt

# Запуск разработческого сервера
python src/backend/main.py

# Использование Kubernetes
kubectl apply -f config/kubernetes/
