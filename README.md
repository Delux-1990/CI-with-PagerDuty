## Задача 3 - интегрировать CI-систему с PagerDuty
# Создать учетную запись в PagerDuty.
```
Aleksandr Sribniy
aleksandr.sribnyi@oceli.energy
```
# Создать пайплайн в любой CI-системе по вкусу.
Пайплайн должен содержать минимум 4 шага: симулировать или выполнять типичный цикл build-test-publish-deploy.
Каждый шаг должен иметь возможность завершиться с ошибкой.
После ошибки на любом шаге дальнейшие шаги не должны выполняться.
Если пайплайн завершается с ошибкой (на любом шаге) - должен случиться триггер инцидента в PagerDuty.
Отправку триггера надо осуществить вручную, прямым обращением в API PagerDuty, без использования готовых интеграций.
# В качестве результата предоставить код пайплайна.
Код пайплайна лежит в файле .gitlab-ci.yml
Проект создан на основе второго задания.
Созданы задачи заглушки, просто чтобы показать, что инциденты создаются, для вызова ошибки нужно раскомментированную строку в .gitlab-ci.yml
# Результат срабатывания триггера
![image](https://user-images.githubusercontent.com/66842337/203714781-efdb9b9c-a324-4a18-b8ff-87668b1cd395.png)


