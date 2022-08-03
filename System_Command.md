# System_Command

#### 1. Check PID
```ruby
pidof python  (vi,nano,apache2)
```
#### 2. Open documentation of command
```ruby
man find  (ls,grep)
```
#### 3. find file which not matching name
```ruby
find ./ -type f -not -name "*.py"
```
#### 4. find file which size less(-) greater(+)
```ruby
find ./ -type f -size +1M
find ./ -type f -size -1M
find ./ -type f -size +1M -size +2M
```
#### 5. Print file name and size (9 and 5 is index of word in ls -lh)
```ruby
find ./ -type f -size +1k -exec ls -lh {} \; | awk '{print $9 "|| size : "$5 }'
```
#### 6. Check runnig services on system
```ruby
systemctl --type service --all | grep running | grep KEYWORD
```
