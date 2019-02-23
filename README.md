# REKKO
https://boosters.pro/championship/rekko_challenge

## Описание
Соревнования по машинному обучению от онлайн-кинотеатра Okko. Обучите рекомендательную систему и предскажите предпочтения пользователей.

## Задача 
На предоставленном тренировочном множестве обучить рекомендательную систему и предсказать топ 20 наиболее релевантных для пользователя идентификаторов контента. Обучающее множество собрано за N дней (N > 60), тестовое множество — за последующие 60 дней.

## Целевая переменная 
В качестве целевой переменной необходимо предсказать множество фильмов, которые пользователь потребил за тестовый период.

Считается, что пользователь потребил контент, если он: 
1. Купил его или взял в аренду 
2. Посмотрел больше половины фильма по подписке 
3. Посмотрел больше трети сериала по подписке

## Формат решения 
Решение должно представлять собой файл формата json, в котором содержится словарь. Ключ словаря — идентификатор тестового пользователя, значение — список из 20 идентификаторов контента, упорядоченные в порядке убывания релевантности.

{ 
  "<user>": [<item_1>, <item_2>, ..., <item_20>], 
  ... 
}
  
