# What is SWR?

SWR stands for stale-while-revalidate, a HTTP cache invalidation strategy popularized by HTTP RFC 5861. It basically means that it performs data fetching in 3 steps:

- Returns cached data first (stale)
- Sends the fetch request (revalidate)
- Returns the up-to-date data

SWR is created by Vercel and one of its advantages is that it is a fast and lightweight package. It is a layer built on top of Fetch API and therefore provides additional features on top of just data fetching. These features include caching, pagination, auto revalidation and more.

## Why use SWR?

1. **Built-in Cache + Real-Time Experience** <br>
When we use Fetch or Axios for data fetching in React, we usually need to show the user some loading message or spinner while data is being fetched. Using SWR’s strategy, the user sees the cached (stale) data first and requests are automatically being cached. Components will always be constantly updated with the most recent data, ensuring UI will always be fast and reactive.

2. **Auto Revalidation** <br>
SWR ensures that the user sees the most up-to-date data. So even with multiple tabs or windows, the data is always fresh and in sync when the window/tab is refocused.

```
import useSWR from 'swr'

function Profile() {
  const { data, error, isLoading } = useSWR('/api/user', fetcher)

  if (error) return <div>failed to load</div>
  if (isLoading) return <div>loading...</div>
  return <div>hello {data.name}!</div>
}
```

In this example, the useSWR hook accepts a key string and a fetcher function. key is a unique identifier of the data (normally the API URL) and will be passed to fetcher. fetcher can be any asynchronous function which returns the data, you can use the native fetch or tools like Axios.

The hook returns 2 values: data and error, based on the status of the request.