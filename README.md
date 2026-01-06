# 🎬 Kasih Review - Backend Service

> **Tugas Besar Implementasi Algoritma (IMPAL)**
> Backend service untuk aplikasi "Kasih Review", dibangun menggunakan Java Spring Boot dan Docker.

![Java](https://img.shields.io/badge/Java-17%2B-orange?style=for-the-badge&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.0-green?style=for-the-badge&logo=spring)
![Docker](https://img.shields.io/badge/Docker-Available-blue?style=for-the-badge&logo=docker)

## 📋 Deskripsi Project
Repository ini berisi *source code* backend (API) untuk aplikasi Kasih Review. Aplikasi ini dirancang untuk memberikan ulasan film, di mana layanan ini menangani logika bisnis, koneksi database, dan autentikasi pengguna.

## 🛠️ Tech Stack
* **Language:** Java
* **Framework:** Spring Boot
* **Build Tool:** Maven (menggunakan Maven Wrapper `mvnw`)
* **Containerization:** Docker & Docker Compose
* **Database:** (Sesuaikan, misal: MySQL / PostgreSQL)

## 📂 Struktur Folder
* `/src` - Source code utama aplikasi (Controller, Service, Repository).
* `Dockerfile` - Konfigurasi image untuk deployment container.
* `docker-compose.yml` - Orkestrasi container untuk menjalankan aplikasi dan database sekaligus.
* `pom.xml` - Manajemen dependensi Maven.

## 🚀 Cara Menjalankan (Getting Started)

Kamu bisa menjalankan aplikasi ini menggunakan dua cara: **Docker** (Direkomendasikan) atau **Manual (Local)**.

### Cara 1: Menggunakan Docker (Paling Mudah)
Pastikan Docker Desktop sudah menyala.

1.  Build dan jalankan container:
    ```bash
    docker-compose up -d --build
    ```
2.  Aplikasi akan berjalan di `http://localhost:8080`.
3.  Untuk mematikan server:
    ```bash
    docker-compose down
    ```

### Cara 2: Menjalankan Manual (Tanpa Docker)
Pastikan Java JDK dan Maven sudah terinstall.

1.  Install dependencies:
    ```bash
    ./mvnw clean install
    ```
2.  Jalankan aplikasi:
    ```bash
    ./mvnw spring-boot:run
    ```

## 🧪 Testing
Untuk menjalankan unit testing yang tersedia di folder `src/test`:
```bash
./mvnw test
