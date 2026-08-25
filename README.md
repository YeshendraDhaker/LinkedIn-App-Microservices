# LinkedIn System — Spring Boot Microservices

> **How LinkedIn searches 900 million jobs & profiles in milliseconds** — built with Spring Boot, Kafka, Elasticsearch, Redis, JWT Authentication and AWS S3.

<br/>

## 📺 Full Video Tutorial

[![LinkedIn App](https://img.shields.io/badge/YouTube-Watch%20Full%20Tutorial-red?style=for-the-badge&logo=youtube)](https://youtu.be/K-EmCZWoCGA)

Watch the complete step-by-step breakdown on YouTube — **free**.

<br/>

## 📦 Get the Source Code

> The complete source code with JWT Authentication, all 6 microservices, Docker Compose, Postman collection and setup guide is available here:

### 👉 [Get Source Code](https://topmate.io/yeshendradhaker/2266876)

**What's included:**
- ✅ Complete source code — all 6 production grade microservices
- ✅ JWT Authentication + Spring Security + BCrypt
- ✅ Elasticsearch full text search — people, skills, posts
- ✅ Fan-out Feed pattern with Redis cache
- ✅ Kafka event driven architecture — 7 topics
- ✅ AWS S3 — profile photos + post images
- ✅ API Gateway — JWT validation + rate limiting
- ✅ Docker Compose — one command setup
- ✅ Postman collection for testing
- ✅ README with complete setup guide

<br/>

## 🐳 Docker Compose (Free)

The infrastructure setup file (MySQL, Redis, Elasticsearch, Kafka, Zookeeper) is available for free:

[![Docker Compose](https://img.shields.io/badge/Google%20Drive-Download%20Docker%20Compose-blue?style=for-the-badge&logo=googledrive)](https://drive.google.com/drive/folders/1O-ZepSk5PPlfRZearc38do3D1WUV9qS1?usp=sharing)

<br/>

## 🏗️ Architecture

```
Client → API Gateway (JWT validation + rate limiting)
              ↓
    ┌─────────┼──────────┬──────────┬──────────┐
    ↓         ↓          ↓          ↓          ↓
 User      Post       Feed      Search   Notification
Service   Service    Service   Service    Service
 8081      8082       8083      8084       8085
 MySQL     MySQL      Redis   Elastic      Kafka
 JWT       AWS S3    Cache     search    consumers
```

<br/>

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Spring Boot 3.2 | Backend framework |
| Apache Kafka | Event driven communication |
| Elasticsearch 8.x | Full text search |
| Redis | Feed caching |
| MySQL | Persistent storage |
| AWS S3 | Media storage |
| JWT + BCrypt | Authentication |
| Spring Cloud Gateway | API Gateway |
| Docker + Docker Compose | Containerization |
| OpenFeign | Service to service calls |

<br/>

<br/>

## 🗄️ Services & Ports

| Service | Port | Database |
|---|---|---|
| API Gateway | 8080 | Redis (rate limiting) |
| User Service | 8081 | MySQL |
| Post Service | 8082 | MySQL + AWS S3 |
| Feed Service | 8083 | Redis only |
| Search Service | 8084 | Elasticsearch only |
| Notification Service | 8085 | Stateless |

<br/>

## 📚 Full Microservices Series

| Project | Link |
|---|---|
| 🎬 Netflix Clone | [Watch on YouTube](https://youtu.be/zY7gSNJ-WuU) |
| 🚗 Uber Clone | [Watch on YouTube](https://youtu.be/Cdx4DF9N8d8) |
| 🏦 Digital Banking System | [Watch on YouTube](https://youtu.be/7Upc4iCsSh4) |
| 💼 LinkedIn System | This video |

<br/>

## 👨‍💻 Connect

| Platform | Link |
|---|---|
| YouTube | [@YeshendraDhaker](https://www.youtube.com/@YeshendraDhaker) |
| LinkedIn | [Yeshendra Dhaker](https://www.linkedin.com/in/yeshendra-dhaker-8b3ab0254) |
| Career Guidance | [Topmate](https://topmate.io/yeshendradhaker) |

<br/>

---

> ⭐ **Star this repo** if it helped you understand microservices architecture!
> 
> 🔔 **Subscribe** to the YouTube channel for more production grade projects.
