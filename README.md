# simple-devops-pipeline
## Proje Akışı

1. **Docker Run**
   - Uygulama ilk olarak `docker run` ile manuel şekilde çalıştırıldı.

2. **Docker Compose**
   - Daha sonra Docker Compose kullanılarak container yönetimi kolaylaştırıldı.

3. **Self-Hosted CI/CD**
   - Son aşamada GitHub Actions self-hosted runner kuruldu.
   - `main` branch’e yapılan her `git push` sonrası:
     - Docker image oluşturulur
     - Docker Hub’a gönderilir
     - Docker Compose ile otomatik olarak deploy edilir

Yapılan değişiklikler http://localhost:8080/ adresinden anlık olarak takip edilmiştir.
