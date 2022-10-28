# createCorrectionOrder
* Позволяет передать данные о корректировке заказа (добавить или удалить данные строк заказа)
* Пример текста пакета:
```json
{
    "Какой-то пример": "Пример"
}
```

* Корневой элемент: **createCorrectionOrderRequest**
    * Множественность: запрещена
    * Вхождение: 1
    * Обязательный: да

## createCorrectionOrderRequest
* Элементы:
    * **CorrectionOrder**
        * Тип: [CorrectionOrder](#correctionorder)
        * Множественность: запрещена
        * Вхождение: 1
        * Обязательный: да

## CorrectionOrder
* Элементы:
    * **Order**
        * Тип: [Order](#order)
        * Множественность: запрещена
        * Вхождение: 1
        * Обязательный: да
    * **Doc**
        * Тип: [Doc](#doc)
        * Множественность: запрещена
        * Вхождение: 1
        * Обязательный: да
    * **CorrectionRows**
        * Тип: [CorrectionRow](#correctionrow)
        * Множественность: разрешена
        * Вхождение: unbounded
        * Обязательный: да

## Order
* Элементы:
    * **Stock**
        * Тип: Stock
        * Множественность: запрещена
        * Вхождение: 1
        * Обязательный: нет

* Атрибуты:
    * **OrderID**
        * Тип: string
        * Обязательный: да
    * **OrderNum**
        * Тип: string
        * Обязательный: нет
    * **TaskID**
        * Тип: string
        * Обязательный: нет
    * **OrderDate**
        * Тип: int
        * Обязательный: нет
    * **DocTypeID**
        * Тип: int
        * Обязательный: нет
    * **Comment**
        * Тип: string
        * Обязательный: нет
    * **StatusID**
        * Тип: string
        * Обязательный: нет

<!-- ## Doc
* Элементы:
    * **Order**
        * Тип: Order
    * **Doc**
        * Тип: Doc
    * **CorrectionRows**
        * Тип: CorrectionRow

## CorrectionRow
* Элементы:
    * **Order**
        * Тип: Order
    * **Doc**
        * Тип: Doc
    * **CorrectionRows**
        * Тип: CorrectionRow -->