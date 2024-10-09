# SWE_2021_41_2024_2_week_6
---
## Week 4 Assignment
- [Week4](https://github.com/slllldka/SWE_2021_41_2024_2_week_4 "Week4 Repository Link")
```python
def isHappy(n):
  numset = set()

  while not n in numset:
    sum = 0
    for x in list(str(n)):
      sum += int(x)*int(x)
    if sum == 1:
      return True
    numset.add(n)
    n = sum
  return False
```
- Get n as a parameter
- Create a empty set
- iterate until n is not in a set
  - calculate sum of each digit's square
  - if sum is 1 then return True
  - add n to numset
  - reassign n to sum

- when exited the while loop, return False

---
## Week 5 Assignment
><pre>
>  <code>docker exec ossp-container cat /etc/os-release</code>
></pre>
> - show os information of docker container

><pre>
>  <code>docker exec ossp-container git --version</code>
></pre>
> - show git version of docker container

><pre>
>  <code>docker exec ossp-container python3 --version</code>
></pre>
> -show python 3 version of docker container

><pre>
>  <code>docker inspect --format="{{ .HostConfig.Binds }}" ossp-container</code>
></pre>
> -show list of bind mounts of docker container
