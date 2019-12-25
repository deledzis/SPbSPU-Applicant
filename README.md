# SPbSPU Applicant

## Проблема
В настоящее время все большая часть  основного трафик пользователей приходится на приложения. На данный момент у Политеха нет своего собственного приложения, которое могло бы познакомить абитуриентов со структорой университета.

## Преимущества
* Работа в офлайн режиме
* Быстрый доступ к структуре университета, расписание приемной кампании, список наиболее частых вопросов и ответов на них
* Карта со всеми корпусами и общежитиями университета, в том числе с указанием тех, в которых ведется прием документов
* Удобный доступ к документации приемной кампании.

## Архитектура
Приложение написано на языке Kotlin с использованием Android SDK. Приложение состоит из одного главного модуля. Написано с использованием паттерна проектирования Android приложений SAA - Single Activity Approach, т.е. приложение состоит из одного главного MainActivity, которое управляет подключёнными к нему фрагментами.
Структурно проект разбит на базовые классы, а также feature-пакеты, содержащие реализации отдельных фундаментальных элементов приложения (экран таймлайна, экран карты, экран структуры университета, экран меню с ЧаВо).

## Тестирование
Данное приложение мы протестировали при помощи ручного тестирования, а точнее опробовали приложение на устройствах с разными версиями Android, начиная с Android 4.4 (SDK 19) и до Android 9.0 (SDK 28). Также было произведено Usability тестирование.

## Сборка
Для сборки проекта используется система сборки Gradle. Артефактом процесса сборки является APK файл.

Команда для сборки, например, APK с debug подписью (не предназначенной для релиза в Play Market) в Windows:
```
gradlew assembleDebug
```
в MacOS:
```
./gradlew assembleDebug
```

## Установка и Запуск
В корне проекта лежит собранный APK файл подписанный дебажным ключом `spbspu-applicant.apk`. Данный файл необходимо запустить на Android устройстве, после чего установить, а также предоставить разрешения на установку, если потребуется.

## Дополнительно. Демонстрация работы
[Скринкаст с демонстрацией работы приложения](https://github.com/deledzis/SPbSPU-Applicant/blob/master/screencast/screencast.mp4)
