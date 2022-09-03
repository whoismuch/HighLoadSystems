# Лабораторная работа №1

### Состав: 
Байрамова Хумай P34312 <br>
Лисицина Василиса P34312

## Предметная область: Интернет-магазин попитов

### Пример архитектуры БД:

```mermaid
   classDiagram
   AntistressToy "*" <-- "1" Production 
   Order "1" --> "*" AntistressToy
   Role "1" --> "*" User
   User "1" --> "*" Client
   User "1" --> "*" Deliveryman
   StressType "*" <--> "*" AntistressToy 
   Client "1" -- "1" Order
   Order "1" -- "1" DeliveryAct
   DeliveryAct "1" -- "1" Deliveryman
```

