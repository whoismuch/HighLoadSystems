# Лабораторная работа №1

### Состав: 
Байрамова Хумай P34312 <br>
Лисицина Василиса P34312

## Предметная область: Интернет-магазин попитов

### Пример архитектуры БД:

```mermaid
   classDiagram
   AntistressToy "*" <-- "1" Production 
   ShoppingCart "1" --> "*" AntistressToy
   Order "1" --> "*" ShoppingCart
   Role "1" --> "*" Client
   Role "1" --> "*" Deliveryman
   Person "1" -- "1" Client
   Person "1" -- "1" Deliveryman
   StressType "*" <--> "*" AntistressToy 
   Client "1" -- "1" Order
   Order "1" -- "1" DeliveryAct
   DeliveryAct "1" -- "1" Deliveryman
```

