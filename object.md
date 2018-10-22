**Object Retuns**

Ruby gives you a keyword for making return values explicit: return. The use of this
keyword is usually optional, but many programmers like to use it because it makes
explicit what is otherwise implicit:
```ruby
def obj.c2f(c)
 return c * 9.0 / 5 + 32
end
```


**Example**
```ruby
class Box

end
box = Box.new

def box.date
    "01/02/03"
end

def box.first_address
    "Town Hall"
end

def box.name
    "Author's reading"
end

def box.second_name
    "Mark Twain"
end

def box.full_address
    "Second Balcony, row J, seat 12"
end

def box.price
    "$5.50"
end   
puts "Complete Address : #{box.date}
#{box.first_address} 
#{box.name}
#{box.second_name}
#{box.full_address}
#{box.price}"
```
**Output:**
```ruby
Complete Address : 01/02/03
Town Hall 
Author's reading
Mark Twain
Second Balcony, row J, seat 12
$5.50
```
**Identifying objects uniquely with the object_id method**
```ruby
strin_1 = "abc"
strin_2= "abc"
puts "The valueof #{strin_1.object_id} and #{strin_2.object_id}"
```
```ruby
The valueof 46959069069400 and 46959069069380
```

Even though these two strings contain the same text, they aren’t, technically, the same
object. If you printed them out, you’d see the same result both times ("Hello"). But
the string objects themselves are different. It’s like having two copies of the same
book: they contain the same text, but they aren’t the same thing as each other. You
could destroy one, and the other would be unaffected. 

    
