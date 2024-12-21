# Контрольные вопросы

## Задача классификации
**Задача классификации** заключается в определении категории (класса), к которой относится объект, на основании его характеристик. В отличие от регрессии, результатом классификации являются дискретные значения.

### Примеры задач классификации:
1. Классификация писем как спам или не спам.
2. Определение породы собаки по фотографии.
3. Диагностика заболеваний на основании медицинских показателей.
4. Прогнозирование, будет ли клиент платить по кредиту (одобрение/отказ).

---

## Что такое шаг градиентного спуска?
**Шаг градиентного спуска** — это величина, на которую обновляются параметры модели на каждой итерации оптимизации. Размер шага зависит от скорости обучения, которая контролирует, насколько быстро модель приближается к оптимальному решению.

- **Маленький шаг:** процесс оптимизации медленный, но стабильный.
- **Большой шаг:** процесс быстрый, но может быть нестабильным или не привести к решению.

---

## Какая функция используется в качестве функции ошибки в модели логистической регрессии?
В логистической регрессии используется **логистическая функция потерь**, также называемая **кросс-энтропией**. Она измеряет разницу между предсказанными вероятностями и фактическими метками классов. 

Эта функция ошибки эффективно штрафует модель за неправильные и слишком уверенные предсказания, что помогает улучшить качество классификации.

---

## Зачем при реализации логистической регрессии к матрице признаков добавлялся столбец из единиц?
Столбец из единиц добавляется для учета **свободного члена** в модели. Свободный член позволяет модели смещать разделяющую границу, чтобы она лучше подходила под данные. 

Без этого добавления модель была бы ограничена в гибкости и не могла бы корректно учитывать случаи, где данные нельзя разделить через начало координат.