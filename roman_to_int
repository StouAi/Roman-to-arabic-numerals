def romanToInt(s):
    sum=0
    slist=list(s)
    complist=[]
    num_dict={'I':1,'V':5,'X':10,'L':50,'C':100,'D':500,'M':1000}
    num_comb={'IV':4,'IX':9,'XL':40,'XC':90,'CD':400,'CM':900}
    for x in slist:
        complist.append(x)
        if len(complist)==2:
            compkey=''.join(complist)
            if compkey in num_comb.keys():
                sum+=num_comb.get(compkey)
                print(complist)
                complist=[]
            else:
                sum+=num_dict.get(complist[0])
                complist[0]=complist[1]
                del complist[1]
    if len(complist)!=0:
        sum+=num_dict.get(complist[0])
    return sum
