# Поиск объекта на изображении по шаблону 
> *Выполнила команда №5: **Набатов Арсений, Ян Цзяфэн, Власенко Наталия, Бурдаев Игорь, Сёмочкин Владимир***

## Подробное задание
https://github.com/IlyaMukhametyanov/cv_lab_2

## Описание решений
### Ключевые точки
Ключевые точки – углы объектов или точки с резким перепады цвета. 

На оригинальном и шаблонном изображении производится поиск ключевых точек, после чего они сопоставляются и лучшее совпадение является найденным объектом. 

### Поиск шаблона по пикселям
Идея состоит в том, чтобы обработать шаблон и довести его до естественного вида объекта, присутствующего непосредственно на изображении оригинала.

Изображение с шаблоном было повёрнуто и обрезано. После чего уже использовался метод поиска шаблона по пикселям.

## Решения
Задача была решена 2 способами: 
1. Поиск ключевых точек
2. Поиск шаблона по пикселям

| Метод | Ср. IoU |
| ------ | ------ |
| [ORB 1](https://colab.research.google.com/drive/11f65zVX6kSmL52E_NNUfLTDBiqaQTZyK?usp=sharing) | 0.343 |
| [ORB 2](https://colab.research.google.com/drive/13jqZQ7p70qIntkSUGUXsGauNWnQIPw3m?usp=sharing) | 0.343? |
| [SIFT](https://drive.google.com/file/d/1vAUR2EFW6dYKFVW_VDfsgkfQZXvmIMu1/view?usp=sharing) | 0.422 |
| [Совпадение пикселей](https://colab.research.google.com/drive/1PWNlBoW1pJIoeSbfGaRHm4ZbgH_bUm63?usp=sharing) | 0.936 |

## Картинки
### ORB 1

![image](https://github.com/4graf/search_pattern_in_image/assets/49661732/aa7cf78d-c103-40e2-821e-7fbfa12e85e2)
![image](https://github.com/4graf/search_pattern_in_image/assets/49661732/c6b45218-3ea3-46d7-8b93-8ea82d793e7f)

### SIFT 

![image](https://github.com/4graf/search_pattern_in_image/assets/49661732/e9eab101-738c-4427-b9b6-f73f60dffec0)

### Совпадение пикселей

![image](https://github.com/4graf/search_pattern_in_image/assets/49661732/62375b0e-d739-4fe3-bd47-4a1708b45250)
![image](https://github.com/4graf/search_pattern_in_image/assets/49661732/87fe73b7-23d2-4a58-8734-0800c21f9cf2)
