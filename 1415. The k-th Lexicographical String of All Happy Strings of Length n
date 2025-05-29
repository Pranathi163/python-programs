class Solution:
    def getHappyString(self, n: int, k: int) -> str:
        q=collections.deque()
        res=[]
        q.append('a')
        q.append('b')
        q.append('c')
        while q:
            ele=q.popleft()
            if len(ele)==n:
                res.append(ele)
                continue
            if ele[-1]=='a':
                first=ele+'b'
                second=ele+'c'
            elif ele[-1]=='b':
                first=ele+'a'
                second=ele+'c'
            else:
                first=ele+'a'
                second=ele+'b'
            q.append(first)
            q.append(second)
        if k>len(res):
            return ""
        return res[k-1]
            



