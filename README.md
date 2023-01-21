# Расстановка типовых секций жилых домов в Autodesk Autocad

## Исходные данные данные

От САПР приходят данные о расстановке типовых секций жилых домов на земельном участке.

```python
  # Координаты границ участка
  323.2 107.8
  155.2 110.8
  134.2 131.2
  ...
  
  # Координаты всех секций на участке
  (122, 249), (152, 271)
  (152, 246), (182, 268)
  (183, 243), (213, 265)
  (213, 240), (243, 262)
  ...
  
  # Коэфициент масштаба (сколько метров в 1 пикселе)
  0.6555517674844418
```
Визуально это выглядит так:

![Расстановка секций, полученная от САПР АРХИП](https://github.com/atiksorg/arhip_autocad_task/blob/main/arhip_area_result.png)

В Autocad мы имеем 2 типовые секции (вертикальную и горизонтальную):

![Типовые секции в Autocad](https://github.com/atiksorg/arhip_autocad_task/blob/main/autocad_sections.png)

## Постановка задачи

### Сгенерировать файл в формате .DWG в котором типовые секции были расположены на участке по данным из САПР АРХИП.

Вот пример результата работы:

![Резельтат расстановки типовых секций по данным из САПР АРХИП в Autocad](https://github.com/atiksorg/arhip_autocad_task/blob/main/autocad_result.png)

### [DWG файл](https://github.com/atiksorg/arhip_autocad_task/blob/main/47.21.0301005.13.dwg)

### Требования к разработке

- Python 100%
  - Версия не ниже 3.7.2
  - Рекомендуемые библиотеки:
    - win32com.client
    - pythoncom
    - pyautocad
- Версия Autocad 2018
