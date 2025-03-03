# Big_data_Kafka
## Лабораторная работа 1. Kafka
В этой лабораторной работе мы настроим окружение для работы с Apache Kafka, создадим простой пайплайн для сбора, обработки и анализа данных с использованием Python. Мы также выполним визуализацию данных.         
Настроить окружение.         
Найти или сгенерировать датасеты.         
Имитировать сбор данных.         
Обработка данных, препроцессинг         
Анализ данных с помощью ML/DL        
Визуализация           
### Шаг 1: Настройка окружения
#### 1) Установка Apache Kafka
Скачайте Apache Kafka с официального сайта. Распакуйте архив и перейдите в директорию Kafka.          
Запустите Zookeeper и Kafka.

```
bin/zookeeper-server-start.sh config/zookeeper.properties
bin/kafka-server-start.sh config/server.properties
```

#### 2) Установка модуля Python

```
pip install kafka-python
```

### Шаг 2: Создание топика в Kafka

```
bin/kafka-topics.sh --create --topic sensor-data --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
```
