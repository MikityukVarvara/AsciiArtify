| Команда                                               | Пояснення                                                                                    |
|-------------------------------------------------------|----------------------------------------------------------------------------------------------|
| `kubectl cluster-info`                                | Команда виводить інформацію про кластер Kubernetes, таку як адреса сервера та версія API.      |
| `kubectl get all -A`                                 | Команда виводить інформацію про всі ресурси (підсистеми, служби, залишки, тощо) у всіх просторах імен. |
| `kubectl create namespace argocd`                     | Команда створює новий простір імен з назвою "argocd".                                      |
| `kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml` | Команда застосовує конфігураційні файли з GitHub репозиторію ArgoCD для розгортання ArgoCD у створеному просторі імен "argocd". |
| `kubectl get pods -n argocd -w`                       | Команда виводить список всіх поточних підсистем (подій) у просторі імен "argocd" і відслідковує їх. |
| `kubectl port-forward svc/argocd-server -n argocd 8080:443` | Команда налаштовує пряме з'єднання (port forwarding) зі службою "argocd-server" у просторі імен "argocd" на порт 8080 на локальному комп'ютері. |
| `kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}"\|base64 -d;echo` | Команда отримує пароль адміністратора ArgoCD, який зберігається у секреті "argocd-initial-admin-secret" у просторі імен "argocd", та розшифровує його з base64 формату. |

![argo](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/a8da3f4f-6c48-4616-9fc8-59da61b1cdc9)


![1](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/93b73007-b90b-4cd8-9c25-f45e582550ea)
![2](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/07e6f4e6-cbeb-47f6-a895-f95fce6701d5)
![3](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/191a59ca-4f35-4ee2-b48c-ec74aca8210e)
![4](https://github.com/MikityukVarvara/AsciiArtify/assets/75087866/76eeff6b-2f36-4e76-8790-af13f490466e)
