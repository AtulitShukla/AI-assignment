# AI-assignment
st1="I am a human being"
st2="I am good"
st3="Good graders study well"
st4="Humans love graders"
st5="Every human does not study well"
st_5="Every human study well"
count=0
result=0
tval=[[1,1],[1,0],[0,0],[0,1]]
for value in tval:
    if value[0]==1:
        st3="T"
    else: 
        st3="F"
    if value[1]==1:
        st5="T"
    else:
        st5="F"
    if st5=="T":
        st_5="F"
    else:
        st_5="T"

    for i in (st3 and st5):
        if i=="T":
            count+=1
if count==len(tval):
    result="YES"
else:
    result="NO"
print("Is every human is a good grader? :   ",result)
