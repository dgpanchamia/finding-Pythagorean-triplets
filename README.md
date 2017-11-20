# finding-Pythagorean-triplets
#The program in pythong 3.x to find integer sides of right angle triangle below given limit
limit=int(input('enter upper limit'))
w,m=0,2
count=0
while(w<limit):
  for n in range(1,m+1):
    p=m*m-n*n
    q=2*m*n
    w=m*m+n*n
    if(p==0 or q==0 or w==0):
      break
    print(p,q,w)
    count+=1
  m=+1
print(count)
