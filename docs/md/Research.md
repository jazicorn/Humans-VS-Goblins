## Notes
> research; planning;

#### Project Extra's Product Tool Brainstorming
1. human has inventory system
   - use interface for different type of items
   - game devs say json/no-sql database is best for inventory database
   - [redis](https://redis.com/solutions/industries/gaming/)
   - [redisJSON](https://redis.com/modules/redis-json/)
   - inventory system module contains:
     - item files
     - user inventory files
     - connection to redisJSON database
2. goblins have drops
   - Different drops random rates
   - [loot drop best practices](https://www.gamedeveloper.com/design/loot-drop-best-practices)
   - [designing-drop-table](https://www.quora.com/What-goes-into-designing-a-random-loot-drop-system-in-a-video-game-Is-it-complex)
   - when goblin dies player has chance receive items
3. stats can be modified by equipment
   - equipment contains combat values
4. map generate random treasure chest after each round of combat
    - Math.Random to generate chest on map grid
5. goblins pursue player
    - Ask Instructor how this is supposed to work
6. Keep track of player score
   - create a scoreboard for top players
   - [redis-leaderboard](https://redis.com/solutions/use-cases/leaderboards/)
   - Use a Hash to store multiple values
     > You can create a dataset that can be sliced by numerous variables. 
     > To do so, it’s helpful to store data in a structure that represents each competitor. 
     > Redis provides just such a structure, called a Hash.
     > A Hash can hold numerous name-value pairs that are associated with one key.
   - Use Timeseries for updating
     - [redis-timeseries](https://redis.com/modules/redis-timeseries/) 
     - [unlocking-timeseries](https://redis.com/blog/unlocking-timeseries-data-redis/)
     - [site](https://oss.redis.com/redistimeseries/)
     - [github-redis-timeseries-libraries](https://github.com/redistimeseries)
 
#### Topics  
- topic: session store
    > A session store is a set of data that connects a user to a service, allowing information to be persisted without having to constantly access the primary database.

#### redis products:
1. [redisBloom](https://redis.com/modules/redis-bloom/)
    - Low latency and compact probabilistic data structures for Redis
    - RedisBloom provides Redis with support for additional probabilistic data structures. These structures allow for constant memory space and extremely fast processing while still maintaining a low error rate. It supports scalable Bloom and Cuckoo filters to determine whether an item is present or absent from a collection with a given degree of certainty, Count-min sketch to count the frequency of the different items in sub-linear space, and Top-K to count top k events in a near deterministic manner.
2. [redisJSON](https://redis.com/modules/redis-json/)
    - RedisJSON is a high-performance NoSQL document store that allows developers to build modern applications. It provides native APIs to ingest, index, query, and run full-text search on JSON documents both on-premises and as a managed service in the cloud.
3. [redis-timeseries](https://redis.com/modules/redis-timeseries/)
    - RedisTimeSeries simplifies the use of Redis for time-series use cases like IoT, stock prices, and telemetry.
    - With RedisTimeSeries, you can ingest and query millions of samples and events at the speed of Redis. Advanced tooling such as downsampling and aggregation ensure a small memory footprint without impacting performance. Use a variety of queries for visualization and monitoring with built-in connectors to popular tools like Grafana, Prometheus, and Telegraf.
4. [redis-graph](https://redis.com/modules/redis-graph/)
    - Fast graph processing powered by linear algebra and matrix multiplication
    - RedisGraph is based on a unique approach and architecture that translates Cypher queries to matrix operations executed over a GraphBLAS engine. This new design allows use cases like social graph operation, fraud detection, and real-time recommendation to be executed 10x – 600x faster than any other graph database.
5. [redis-messaging](https://medium.com/snipe-gg/3-ways-we-use-redis-to-make-gaming-awesome-7c1a74905bd2)
  - ***purpose***
    - Modern software applications have moved from being a single monolithic unit to loosely coupled collections of services. While this new architecture brings many benefits, those services still need to interact with each other, creating the need for robust and efficient messaging solutions.
  - ***messaging services:***
      1. **Redis Streams** doubles as a communication channel for building streaming architectures and as a log-like data structure for persisting data, making Streams the perfect solution for event sourcing.
      2. **Redis Pub/Sub** is an extremely lightweight messaging protocol designed for broadcasting live notifications within a system. It’s ideal for propagating short-lived messages when low latency and huge throughput are critical.
      3. **Redis Lists and Redis Sorted Sets** are the basis for implementing message queues. They can be used both directly to build bespoke solutions, or via a framework that makes message processing more idiomatic for your programming language of choice.
  - ***message queues?***
      - Message queues are based on mutable lists and are sometimes consumed through tools that help implement common patterns. There are two main differences between message queues and event streams: Message queues use a “push” type of communication—a service pushes a new message to another service’s inbox whenever something new needs attention. Streams operate in the opposite way.
      - Messages contain mutable state (e.g., number of retries) and, when successfully processed, they are deleted from the system. Stream events are immutable and the history, when trimmed, is often saved in cold storage.
  - ***event streams***
      - Event streams are based on the log data type, which is extremely efficient at seeking through its history and appending new items to its end. These two properties make the immutable log both a great communication primitive, and an efficient way to store data.
      - Communicating through a stream is different than using a message queue. As mentioned previously, message queues are “push,” while streams are “pull.” In practice, this means that each service writes to its own stream and other services will optionally observe (i.e. “pull” from) it. This makes one-to-many communication much more efficient than with message queues.

#### Possible Docker + Jenkins Configuration
Steps are the following:
- Develop the microservice
- Define the build process in which the service will be dockerized
- Use GitHub for hosting the Git code repository
- Integrate GitHub with Jenkins to package the application using Gradle
- Push it to a remote Amazon ECR

More Steps:
- Spring Boot example application – microservice packaged and dockerized using Gradle
- Jenkins installation on a fresh Ubuntu server
- GitHub integration with Jenkins via webhook
- Jenkins job configuration
- Amazon ECR to store the Docker images containing our application

### API Example
> Product Service provides API to get the product details combined with review details for a specific product
#### Project Details
1. Build RESTFul APIs using @RestController and use of short annotations @GetMapping, @PostMapping, @PutMapping, and @DeleteMapping
2. Service Layer development using @Service to provide business logic to @RestController
3. Global API Exception Handler using ApiExceptionHandler to customize the API response for errors
4. API Documentation using Spring OpenAPI and Swagger configuration using OpenApiConfig
5. API Logging using ApiLoggingFilterConfig to log API request and response
6. Consume RESTFul APIs provided by other services using @FeignClient
7. Boilerplate Code generation using Lombok annotations such as @Data, @Value, @ToString, @Getters, and @Setters
8. Unit and Integration Tests for Controller and Service Layer