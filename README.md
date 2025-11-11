# mirea-devsecops-lab

Настоящее практическое задание разработано для студентов 1 курса РТУ МИРЭА, обучающихся по программе Элитной подготовки, в рамках цикла лекций по информационной безопасности.
Целью задания является формирование базовых знаний и практических навыков по внедрению принципов безопасной разработки (SSDLC, DevSecOps).

## Подготовка окружения
1. Создать аккаунт на [github.com](https://github.com/) 
2. [Установить git](https://git-scm.com/install/) 
3. Сконфигурировать git:
```console
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```
4. [Создать ssh-ключи](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent),[ добавить их в аккаунт](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account),[проверить доступность](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection)

## Задание:
1. Сделать fork репозитория, затем склонировать локально по ssh.
2. Запустить pipeline: вкладка Actions → Security Checks → кнопка Run workflow. Pipeline запустится и упадёт.
3. Просмотреть результаты проверок (Semgrep/Trivy) и найти причину failure.
4. Найти уязвимости в коде и исправить их.
5. Запушить изменения и убедиться, что pipeline проходит.