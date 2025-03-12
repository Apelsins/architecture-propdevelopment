Что-то у меня не переходит по ссылке https://code.s3.yandex.net/software-architect/7?etag=dce4ea23a31ae4e92bc43eb90c472668. 
Это ссылка на пример таблицы из задания.

Так что опишу тут.
user1 <-  user1-rolebinding  -> role-1
user2 <-  user2-rolebinding  -> role-2

Команды, которые выполнял:
kubectl apply -f users.yml
kubectl apply -f roles.yml
kubectl apply -f rolebindings.yml

Вот результат, который вызывается командой kubectl get rolebindings -n default
NAME                ROLE          AGE
user1-rolebinding   Role/role-1   5s
user2-rolebinding   Role/role-2   5s

