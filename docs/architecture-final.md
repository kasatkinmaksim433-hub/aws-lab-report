# Фінальна архітектура проекту

* **VPC**: Використовується налаштована мережа з Lesson1_4[cite: 2].
* **Compute**: Два EC2-інстанси (`i-web-a`, `i-web-b`) розгорнуті у різних зонах доступності[cite: 1, 9].
* **Load Balancing**: Application Load Balancer (`my-web-alb`) з цільовою групою `my-web-tg` розподіляє трафік[cite: 1].
* **Storage**: S3-бакет `my-frontend-bucket-maks-2026` для розміщення фронтенду[cite: 1].
* **Обмеження**: Створення CloudFront та Lambda-функцій заблоковано через права навчального середовища (`voclabs`).
