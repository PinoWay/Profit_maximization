# Максимизация экономической прибыли

Имеются данные по займам, а также значения факторов. Необходимо построить скоринговую модель, которая позволит максимизировать совокупную экономическую прибыль. Скориноговая модель должна получать на вход значения фактаров, а на выходе давать ответ, нужно ли выдать данный заем.

Значение экономической прибыли рассчитывается следующим образом:
* Loss = Unpaid * (EL, expected loss)
* InvestorProfit = Earned - Loss
* Profit = InvestorProfit + Commission
* Profit% = Profit / LoanIssued

## Структура репозитория
- data
    - main_data.xlsx - файл с данными о заемщиках
- Modeling.ipynb - ноутбук с анализом данных и моделированием
- final_model.pkl - финальная модель 

## Результаты моделирования
При рассмотрения различных моделей машинного обучения, был получен интересный результат - с данной задаче лучше всего справляется модель решающего дерева. Помимо получения классификатора также были оценены самые важные признаки для определения выдавать заем клиенту или нет (cм. Modeling.ipynb).