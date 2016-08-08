# sorting
hash=Hash.new
puts"How many elements you want to enter"
n=gets.to_i
array=[]
for k in 0...n do
  array.push(gets.to_i)
end

for i in 0...n do
  for j in i...n do
    hash[[i,j]]=array[j]-array[i]
  end
end
puts hash.key(hash.values.max)

