def insertion_sorting(array):
  size=len(array)
  for index in range(1,size):
    pointer=array[index]
    i=index-1
    while i>=0:
      if pointer<array[i]:
        array[i+1]=array[i]
        array[i]=pointer
        i-=1
      else:
        break

array=[9,5,1,4,3]
insertion_sorting(array)
print(array)  