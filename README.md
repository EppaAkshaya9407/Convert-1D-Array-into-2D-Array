# Convert-1D-Array-into-2D-Array
class Solution:
    def construct2DArray(self, original: list[int], m: int, n: int) -> list[list[int]]:
        l=len(original)
        if m*n!=l:
            return []
        res=[]
        c=0
        for i in range(m):
            r=[]
            for j in range(n):
                r.append(original[c])
                c+=1
            res.append(r)
        return res

                
