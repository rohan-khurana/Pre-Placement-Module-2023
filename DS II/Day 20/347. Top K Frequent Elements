class Solution:
    def topKFrequent(self, nums: List[int], k: int) -> List[int]:
        count = {}
        
        for num in nums:
            count[num] = count.get(num, 0) + 1
            
        heap = []
        for key, value in count.items():
            heapq.heappush(heap, (-value, key))
                           
        results = []
        
        for i in range(k):
            count, element = heapq.heappop(heap)
            results.append(element)
                           
        return results
