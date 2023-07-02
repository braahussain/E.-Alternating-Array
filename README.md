a = int(input())
arr = input().split(' ')
mul = -1
ch1,ch2 = 0,0
for i in range(len(arr)) :
    arr[i] = int(arr[i])
    x= abs(arr[i])*mul
    y= abs(arr[i])*-1*mul
    mul*=-1
    if arr[i]!=x : ch1+=1
    if arr[i]!=y : ch2+=1
print(min(ch1,ch2))
