t = int(input())
while t > 0:
    n = int(input())
    arr = list(map(int,input().split()))
    arr.sort()
    arr = arr[::-1]
    sum = 0
    for i in range(n):
        temp = arr[i] - i
        if temp > 0:
            sum += temp
        else:
            break
    ans = sum % 1000000007
    print(ans)
    t -= 1