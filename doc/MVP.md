# РОЗГОРТАННЯ MVP
![3](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/99112020-aac0-4aab-84d4-eb936e8861b0)

## Команди для розгортання додатку
| Команда                                      | Пояснення                                                                                                  |
|----------------------------------------------|------------------------------------------------------------------------------------------------------------|
| kubectl get svc -n demo                      | Команда виводить інформацію про служби (services) у просторі імен `demo`.                                 |
| kubectl port-forward -n demo svc/ambassador 8081:80 | Команда налаштовує пряме з'єднання (port forwarding) зі службою `ambassador` у просторі імен `demo` на порт 8081 на локальному комп'ютері. |
| curl localhost:8081                          | Команда виконує HTTP запит до локального сервера, який слухає на порті 8081.                              |
| wget -O /tmp/g.png https://img2.gratispng.com/20180406/xhq/kisspng-computer-icons-house-window-blinds-shades-brookl-adress-5ac7dd63724750.6622363615230477794681.jpg | Команда завантажує зображення за вказаним URL та зберігає його у файл `/tmp/g.png`.                         |
| curl -F 'image=@/tmp/g.png' localhost:8081/img/ | Команда відправляє POST запит на `/img/` зображенням `g.png` до локального сервера, який слухає на порті 8081. |


### ІНСТРУКЦІЯ ДЛЯ ARGOCD (зображення не завжди описуюють дію або процес)
### 1. **Створення додатку у ArgoCD:** Доданий новий додаток у ArgoCD для відслідковування Git репозиторію продукту за посиланням [https://github.com/den-vasyliev/go-demo-app](https://github.com/den-vasyliev/go-demo-app).
![1](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/5e14910c-991c-4af4-8e38-81cbff9f9013)
![2](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/11cdee88-0cf8-40c5-bb4e-a15ac8838678)
![3](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/ab1f665a-8e08-4b48-ab1a-c03419d2f740)

### 2. **Налаштування автоматичної синхронізації:** ArgoCD налаштований таким чином, щоб автоматично синхронізувати зміни з Git репозиторію та розгортати їх на Kubernetes кластері.
   
![4](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/da1d8e3a-6157-4e3b-988a-64cd83268087)
![5](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/9dfbe9ec-d14c-4466-83ca-1250356d9f8a)
![6](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/ea01fbbf-0c93-4401-9f66-ebdec642dab0)
![7](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/a8473dc1-c74c-48f6-b731-0a8b0b2fa8ac)
![8](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/d540a7cc-04b0-4526-8be6-c24efbf025f0)
### 3.  **Запуск повного циклу демонстрації:** Після успішного налаштування ArgoCD запущений повний цикл, щоб продемонструвати, як він автоматично відслідковує та синхронізує зміни з Git репозиторію та розгортає їх на Kubernetes кластері.
![9](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/4a26b4b3-7d92-4feb-abea-4e44fee061d8)
![10](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/4c11681a-4049-40ee-9c18-6ed2258368c0)

### Детальна інформація описана за посиланням:
https://github.com/vit-um/DevOps/wiki/%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D0%B8-Kubernetes
