# Angular
# DS
# DS Pattern + LeetCode
# Java8 Program
# Java
# Spring Boot
# Microservices
# Database
# Design Pattern
# kafka
# Redis
# Cloud
# Linux
# DevOps
# Docker & K8s
# System Design (FR-NFR(SARCLTS)/HLD/LLD/Security/Monitoring)
# Scenario

**Matrics**
  - Application
    - cpu
    - Memory
    - Thread
    - GC
    - API Latency/error rate
  - DB
    - cpu
    - Connection
    - Query latency
    - Lock
  - Redis
    - Memory
    - Cpu
    - Hit Miss
    - Latency
  - Kakfa
    - Consumer Lag
    - Throughput
    - Partition distribution
    - Broker health


 **Detect**
  - High Error rate
  - High Latency
  - Consumer lag
  - CPU / Memory High
  - DB connection High

**What is the user experiencing?**
  - API 500
  - API Timeout
  - Kafka -> Lag increasing
  - Redis -> High Latecy
  - DB -> Slow Query

**Check logs**
 - ERROR
 - Exception
 - Timeout
 - Connection refused
 - OutOfMemoryError
 - Deadlock
 - Serialization error
 - Authentication failure

**Check Traces**
 - Find where latency or failure starts.

**COMPONENT**
 - Application?
 - DB?
 - Redis?
 - Kafka?
 - Network?
 - External API?
 - Infrastructure?

**ROOT CAUSE**

**IMMEDIATE MITIGATION**
 - Redis failure
 - Kafka consumer lag
 - DB slow

**RECOVER SERVICE**
 - Restart unhealthy pod
 - Failover DB
 - Recover Redis
 - Recover Kafka broker
 - Rollback deployment
 - Scale application
 - Clear stuck processing

**PERMANENT FIX**

**PREVENTION**

**MONITORING / ALERT**
- CPU > 80%
- Memory > 80%
- DB connection pool > 80%
- Kafka lag > threshold
- Redis memory > threshold
- API error rate > threshold
- API latency > threshold

 **Apply Framework to Topics**
  - Kafka Producer | Publish error | Retry/backoff
  - Kafka Consumer | Publish error | Restart/retry
  - Consumer Lag | Lag | Scale consumers
  - Partitioning | Uneven load
  - Replication | Broker/replica failure
  - Retry | Repeated failures
  - Idempotency | Duplicate processing
  - Outbox | DB/Kafka mismatch
  - DLQ/Retry Topic | Repeated failures
    
  - Cache-Aside | High cache miss
  - TTL | Stale/expired cache
  - Stampede | Huge simultaneous misses
  - Penetration | Many nonexistent requests
  - Avalanche | Many keys expire
  - Hot Key | One key overloaded
  - Cache Inconsistency | DB ≠ Redis
    
  - DB Pool
  - Slow Query
  - DB + Kafka
    
  - Redis + Kafka + DB
