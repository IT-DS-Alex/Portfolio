# Определение выгодного региона нефтедобычи

Нам предоставлены пробы нефти в трёх регионах: в каждом 10 000 месторождений, где измерили качество нефти и объём её запасов. Построим модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль. Проанализируем возможную прибыль и риски техникой Bootstrap.

## Шаги для выбора локации:

В избранном регионе ищю месторождения, для каждого определяют значения признаков;
Строю модель и оценивают объём запасов;
Выбираю месторождения с самым высокими оценками значений. Количество месторождений зависит от бюджета компании и стоимости разработки одной скважины;
Прибыль равна суммарной прибыли отобранных месторождений.

![image](https://github.com/IT-DS-Alex/Portfolio/assets/140064630/37df116c-aeff-4810-bdae-3f9d4959a92b)


### Вывод:

Данные загружены и не требуют дополнительной предобработки.

Имеем визуальное представление о распределении данных по запасам сырья в регионах.

На графике показана разительно отличающаяся кривая распределения запасов сырья по скважинам 2 региона.

Отметим так же, что на данных по корреляции значений 2 регоина, мы видим сильную зависимость целевого показателя product от f0, такая зависмость можеть дать нам высокие баллы предсказаний для нашей модели.

![image](https://github.com/IT-DS-Alex/Portfolio/assets/140064630/2a71ba98-83a7-47c4-bab8-d9cadcdf4261)


![image](https://github.com/IT-DS-Alex/Portfolio/assets/140064630/fa64b29b-3c6d-4f2c-88c9-45dc2cf3f7a8)

## Общий вывод:

Были исследованы данные по запасам в скважинах трёх регионов, в каждом из которых были данные о запасах сырья по 10 тыс.скважинам. При первом знакомстве с данными мы обнаружили, что средний запас ресурсов по регионам недостаточен даже для окупаемости вложений на разработку и для того, чтобы иметь уверенность в перспективе разработки по регионам, мы обучили модель и выполнили предсказания при помощи линейной регрессии, а так же применили технологию bootstrap с разделением каждого предсказанного значения прибыли по регионам на 1000 выборок.

По результату полученных данных определил доверительный интревал получения прибыли в 95%, ограничив вероятность убытка величиной менее 2,5%. И на основе этих данных смог выбрать более перспективный регион для разработки 200 скважин.

Таким образом не смотря на сравнительно меньшие предсказания запасов сырья в 27.75 млн.баррелей (по сравнению с другими регионами), с величиной вероятного возникновения убытка в 1,1%, но с превышающей средней прибылью в 489.66 млн.рублей  сделал выбор в сторону разработки 200 скважин во 2 регионе.


