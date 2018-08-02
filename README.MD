# Outlyer backend recruitment test

Thanks for taking the time to do our backend coding test. The challenge has two parts:

- [A coding test](#coding-test)
- [A few follow-up questions](#follow-up-questions)

## Coding Test

- Write a well structured program which provides an API with the endpoint `/metrics` that returns some system metrics in JSON.

- The program should periodically collect and keep values of the system cpu, memory, disk and network metrics in a registry in memory.

- The program should expose the registry values when an http GET request is made to `/metrics`.

- Example output (minimum expected metrics to collect/send, although more can be added):

```
$ curl localhost:8080/metrics
{
    "sys.cpu": "4.15",
    "sys.mem.active": "8029741056",
    "sys.mem.available": "6602049536",
    "sys.disk.free": "13605457920",
    "sys.disk.used": "76558884181",
    "sys.net.rx": "217003.31",
    "sys.net.tx": "11390.29"
}
```

## Implementation

- The code can be written in any language.

- Metric collection should work on UNIX Operating systems.

- You will be evaluated both on your implementation choices and the quality of your code; so
please ensure code is well structured, extensible, tested, readable, commented etc.

- bonus point: design a solution that can dynamically collect other metrics, for example the ones about services running on your host like nginx or redis etc.

## Submission Guidelines

- Please submit your application as a repository on GitHub.

- Please submit an explanation document for your work addressing all the follow-up questions. This should be no more than 1000 words

- Please let your Outlyer contact know when you've uploaded your solution.

## Follow-up Questions

- Which parts did you spend the most time with?

- How long, in hours, did you spend on the test?

- What did you find to be the most difficult?

- What would you add to your solution if you had more time?

- Why did you choose this programming language ?

- How did you find the test overall? If you have any suggestions on how we can improve the test, we'd love to hear them.
