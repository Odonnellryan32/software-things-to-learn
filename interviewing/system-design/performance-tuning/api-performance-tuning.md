# API Performance Tuning

## Caching
- Cache data that is expensive to compute
- Cache data that is frequently accessed
- Cache data that is not frequently updated
- Cache data that is not sensitive

### Patterns
- **Cache-Aside**: Application code is responsible for reading and writing to the cache. When data is requested, the application first checks the cache. If the data is not found in the cache, the application fetches the data from the database and writes it to the cache.
- **Write-Through**: Application writes data to the cache and the cache writes the data to the database. This pattern ensures that the cache and the database are always in sync.
- **Write-Behind**: Application writes data to the cache and the cache writes the data to the database asynchronously. This pattern improves write performance by reducing the number of writes to the database.
- **Read-Through**: Application reads data from the cache. If the data is not found in the cache, the cache fetches the data from the database and writes it to the cache. This pattern ensures that the cache is always up-to-date with the database.
- **Refresh-Ahead**: Cache pre-fetches data before it expires. This pattern ensures that the cache is always up-to-date with the database.
- **Lazy Loading**: Data is loaded into the cache only when it is requested. This pattern reduces the amount of data that is loaded into the cache.


## Connection Pooling
- Reuse connections to reduce the overhead of establishing new connections
- Limit the number of connections to prevent resource exhaustion.


# Sources 
[API Performance Tuning - Byte Byte Go](https://www.youtube.com/watch?v=zvWKqUiovAM&ab_channel=ByteByteGo)
[Connection Pooling - Stack Overflow](https://stackoverflow.blog/2020/10/14/improve-database-performance-with-connection-pooling/)