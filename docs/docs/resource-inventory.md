# Інвентаризація ресурсів

| Назва ресурсу | Тип | ID | Регіон | AZ | Призначення | Залежності |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `my-web-alb` | Application Load Balancer | `arn:aws:elasticloadbalancing:...` | us-east-1 | us-east-1a/1d | Розподіл трафіку | `my-web-tg`, VPC |
| `my-web-tg` | Target Group | `my-web-tg` | us-east-1 | - | Здоров'я вузлів | EC2 інстанси |
| `i-web-a` | EC2 Instance | `i-0844e32d4e06593c3`[cite: 9] | us-east-1 | us-east-1a[cite: 9] | Веб-сервер 1 | VPC, Subnet |
| `i-web-b` | EC2 Instance | `i-0711b4fbd8b4b8d63`[cite: 9] | us-east-1 | us-east-1d[cite: 9] | Веб-сервер 2 | VPC, Subnet |
| `my-frontend-bucket-maks-2026` | S3 Bucket | `my-frontend-bucket-maks-2026`[cite: 1] | us-east-1 | - | Зберігання frontend[cite: 1] | - |
