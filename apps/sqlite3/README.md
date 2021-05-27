# SQLite 3.35.5
- Full-featured version of SQLite 3.35.5
- 1,326,600 bytes
- 696,778 bytes zipped (if added to Redbean.com, your Redbean is still just a bit over a meg)
- Runs on Linux, MacOS, Windows

## What I've been able to do with it:
- embed it inside a Redbean server
- have Redbean shell out to the host os and unzip it so it can be used by Redbean
- shell out to it via lua to make database calls

### having Redbean extract sqlite on init:
- add this to your .init.lua file then add the .init.lua file back into your Redbean (and add sqlite.com to the Redbean of course)

```
function exists(name)
    if type(name)~="string" then return false end
    return os.rename(name,name) and true or false
end
if exists('sqlite3.35.5.com') then
    print('sqlite3.35.5.com exists')
else
    print('sql.com does NOT exist...try to extract it')
    local extract_result = os.execute('unzip -n redsql.com sqlite3.35.5.com')
    if extract_result == true then
        print('sqlite3.35.5.com successfully extracted')
    else
        print('sqlite3.35.5.com extraction failed:', extract_result)
    end  
end
```

### sample lua code for shelling out to sqlite
```
os.execute("./sqlite3.35.5.com test.db 'create table if not exists names (first, last)' 'delete from names'")

local s = {}
s[#s+1] = '("George","Washington")'
s[#s+1] = '("John","Adams")'
s[#s+1] = '("Thomas","Jefferson")'
s[#s+1] = '("Bob","Sponge")'

os.execute("./sqlite3.35.5.com test.db 'insert into names values " .. table.concat(s,',') .. "'")



local f = io.popen ("./sqlite3.35.5.com test.db '.headers on' '.mode tabs' 'select * from names'")

 for line in f:lines() do
   print(line)
 end -- for loop
   
 f:close()
```
